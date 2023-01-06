<template>
  <section class="quote">
    <div class="quote-content">
      {{ quote.content }}
    </div>
    <div class="quote-info">
      <div class="quote-anime">
        {{ quote.anime }}
      </div>
      <div class="quote-author">
        {{ quote.character }}
      </div>
    </div>
  </section>
</template>

<script>
export default {
  props: ['quote']
}
</script>

<style lang="scss" scoped>
.quote {
  position: relative;
  margin: 0 auto;
  padding: 32px;
  max-width: 720px;

  &-content {
    position: relative;
    font-size: 28px;
    font-weight: 600;
    background-color: var(--dark);
    color: var(--light);
    padding: 48px 32px;
    border-radius: 16px;

    &:before, &:after {
      content: '"';
      color: var(--grey);
      margin: 0px 2px;
    }
  }

  &-info {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    padding: 32px;

    .quote-author, .quote-anime {
      position: absolute;
      padding: 12px 16px;
      font-size: 24px;
      font-weight: 700;
      border-radius: 99px;
      color: var(--light);
      text-align: center;
    }

    .quote-author {
      top: calc(100% - 32px);
      right: 0;
      transform: translateY(-50%);
      background-color: var(--secondary);
    }

    .quote-anime {
      top: 0px;
      left: 0px;
      background-color: var(--tertiary);
      color: var(--dark);
    }
  }
}
</style>