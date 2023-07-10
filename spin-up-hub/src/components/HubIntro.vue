<script>
export default {

}
</script>

<template>
  <div class="hub-intro">
    <div class="columns content-inner is-centered">
      <div class="column is-three-fifths-desktop is-full-mobile">

        <div class="search-box">
          <div class="description">WELCOME TO THE SPIN UP HUB</div>
            <input class="search-input" type="text" placeholder="Explore the fermyverse">
          </div>
        </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.hub-intro {
  // padding: 8rem 1rem 1rem 1rem;
  // display: flex;
  // justify-content: center;
  // align-items: center;
  min-height: 22rem;
  padding-top: 10.5rem;
  padding-bottom: 4.25rem;

  .search-box {
    // width: 60%;
    // max-width: 800px;
    padding: 2.5rem 3.33rem;
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    border-radius: 1.2rem;
    border: 1px solid rgba($lavender, 0.2);
    justify-content: center;
    background: desaturate(darken(rgba($lavender, 0.33), 42.5%), 25%);
    box-shadow: 0px 4px 4px 0px rgba(0, 0, 0, 0.25);

    .description {
      margin-top: 1rem;
      font-size: 1.25rem;
      font-weight: 600;
      padding: 1rem;
      text-align: center;
    }

    .search-input {
      margin-top: 1rem;
      border: none;
      padding: 1rem;
      border-radius: 0.67rem;
      width: 80%;
      background-color: $oxfordblue;
    }
  }
}

@media screen and (max-width:1023px) {
  .hub-intro {
    .search-box {
      width: 90%;
    }
  }
}
</style>
