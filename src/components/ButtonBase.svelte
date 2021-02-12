<script>

</script>

<a href="/" class="ButtonBase ButtonBase--orange"><slot></slot></a>

<style lang="scss">
  .ButtonBase {
    display: flex;
    text-align: center;
    min-width: 108px;
    max-width: 159px;
    height: 48px;
    padding: 12px 32px;
    border-radius: 24px;
    font-weight: 500;

    &--orange {
      color: #fff;
      background-color: #EC4E20;
    }
  }
</style>