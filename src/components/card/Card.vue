<script setup>
import IllustrationHeroIcon from "@/assets/images/IllustrationHeroIcon.vue";
import MusicIcon from "@/assets/images/MusicIcon.vue";
</script>
<template>
  <div class="card">
    <IllustrationHeroIcon class="card__img" />

    <div class="card__content">
      <h3 class="card__title">Order Summary</h3>

      <p class="card__txt">
        You can now listen to millions of songs, audiobooks, and podcasts on any
        device anywhere you like!
      </p>

      <div class="card__pay">
        <div class="card__pay-info">
            <MusicIcon class="card__pay-box-icon" />
          
          <div class="card__pay-order">
            <p class="card__pay-order-plan">Annual Plan</p>

            <span class="card__pay-order-price">$59.99/year</span>
          </div>
        </div>

        <span class="card__pay-change">Change</span>
      </div>

      <button class="card__btn">Proceed to Payment</button>

      <a href="#!" class="card__cancel">Cancel Order</a>
    </div>
  </div>
</template>
<style lang="scss" scoped>
.card {
  max-width: 450px;
  width: 100%;
  height: 650px;
  overflow: hidden;
  border-radius: 15px;
  background: var(--cardBgColor);
  display: flex;
  flex-direction: column;

  &__img {
    width: 100%;
  }

  &__title {
    text-align: center;
    font-weight: 900;
    font-size: 26px;
    color: var(--darkColor);
  }

  &__content {
    padding: 40px 50px;
    display: flex;
    flex-grow: 1;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
  }

  &__pay {
    width: 100%;
    border-radius: 10px;
    background: var(--accentColor);
    padding: 20px 15px;
    display: flex;
    justify-content: space-between;
    align-items: center;

    &-change {
      color: var(--secondaryColor);
      font-weight: 700;
      text-decoration: underline;
      transition: 300ms;
      cursor: pointer;

      &:hover {
        color: var(--secAccentColor);
        text-decoration: none;
      }
    }

    &-info {
      display: flex;
      gap: 15px;
    }

    &-order {
      display: flex;
      flex-direction: column;
      justify-content: space-around;
      
      &-plan {
        font-size: 18px;
        font-weight: 900;
        color: var(--darkColor);
      }
      
      &-price {
        color: var(--secAccentColor);
        font-weight: 500;
      }

      
    }
  }

  &__btn {
    width: 100%;
    background: var(--secondaryColor);
    border: 0;
    outline: 0;
    padding: 15px;
    border-radius: 10px;
    font-weight: 700;
    font-size: 16px;
    color: var(--accentColor);
    cursor: pointer;
    transition: 400ms;

    &:hover {
      background: var(--secAccentColor);
    }
  }

  &__cancel {
    color: var(--secAccentColor);
    font-weight: 900;
    font-size: 14px;
    transition: 400ms;

    &:hover {

      color: var(--darkColor);
    }

  }

  &__txt {
    color: var(--secAccentColor);
    width: 300px;
    text-align: center;
    line-height: 1.6;
  }
}
</style>
