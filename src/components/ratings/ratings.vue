<template>
  <div>ra</div>
</template>

<script>
</script>

<style lang="stylus" scoped>
@import '~common/stylus/variable';
@import '~common/stylus/mixin';

.ratings {
  position: relative;
  text-align: left;
  white-space: normal;
  height: 100%;

  .overview {
    display: flex;
    padding: 18px 0;

    .overview-left {
      flex: 0 0 137px;
      padding: 6px 0;
      width: 137px;
      border-right: 1px solid $color-col-line;
      text-align: center;

      @media only screen and (max-width: 320px) {
        flex: 0 0 120px;
        width: 120px;
      }

      .score {
        margin-bottom: 6px;
        line-height: 28px;
        font-size: $fontsize-large-xxx;
        color: $color-orange;
      }

      .title {
        margin-bottom: 8px;
        line-height: 12px;
        font-size: $fontsize-small;
        color: $color-dark-grey;
      }

      .rank {
        line-height: 10px;
        font-size: $fontsize-small-s;
        color: $color-light-grey;
      }
    }

    .overview-right {
      flex: 1;
      padding: 6px 0 6px 24px;

      @media only screen and (max-width: 320px) {
        padding-left: 6px;
      }

      .score-wrapper {
        display: flex;
        align-items: center;
        margin-bottom: 8px;

        .title {
          line-height: 18px;
          font-size: $fontsize-small;
          color: $color-dark-grey;
        }

        .star {
          margin: 0 12px;
        }

        .score {
          line-height: 18px;
          font-size: $fontsize-small;
          color: $color-orange;
        }
      }

      .delivery-wrapper {
        display: flex;
        align-items: center;

        .title {
          line-height: 18px;
          font-size: $fontsize-small;
          color: $color-dark-grey;
        }

        .delivery {
          margin-left: 12px;
          font-size: $fontsize-small;
          color: $color-light-grey;
        }
      }
    }
  }

  .rating-wrapper {
    padding: 0 18px;

    .rating-item {
      display: flex;
      padding: 18px 0;

      &:last-child {
        border-none();
      }

      .avatar {
        flex: 0 0 28px;
        width: 28px;
        margin-right: 12px;

        img {
          height: auto;
          border-radius: 50%;
        }
      }

      .content {
        position: relative;
        flex: 1;

        .name {
          margin-bottom: 4px;
          line-height: 12px;
          font-size: $fontsize-small-s;
          color: $color-dark-grey;
        }

        .star-wrapper {
          margin-bottom: 6px;
          display: flex;
          align-items: center;

          .star {
            margin-right: 6px;
          }

          .delivery {
            font-size: $fontsize-small-s;
            color: $color-light-grey;
          }
        }

        .text {
          margin-bottom: 8px;
          line-height: 18px;
          color: $color-dark-grey;
          font-size: $fontsize-small;
        }

        .recommend {
          display: flex;
          align-items: center;
          flex-wrap: wrap;
          line-height: 16px;

          .icon-thumb_up, .item {
            margin: 0 8px 4px 0;
            font-size: $fontsize-small-s;
          }

          .icon-thumb_up {
            color: $color-blue;
          }

          .item {
            padding: 0 6px;
            border: 1px solid $color-row-line;
            border-radius: 1px;
            color: $color-light-grey;
            background: $color-white;
          }
        }

        .time {
          position: absolute;
          top: 0;
          right: 0;
          line-height: 12px;
          font-size: $fontsize-small;
          color: $color-light-grey;
        }
      }
    }
  }
}
</style>
