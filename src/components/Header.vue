<template>
  <div>
    <header>
      <div class="left">
        <img src="../assets/img/logo.svg" alt class="logo" />
      </div>
      <div class="center">
        <div class="title">
          <h3 class="top">Inside</h3>
          <h1>Tyler Potts</h1>
          <h3 class="bottom">Mind</h3>
        </div>
      </div>
      <div class="right">
        <label for="sear-bar">
          <img src="../assets/img/search-icon.png" class="icon" />
          <input type="text" id="search-bar" name="search-bar" placeholder="Type to search..." />
        </label>
      </div>
    </header>
  </div>
</template>
<script>
export default {
  name: "header"
};
</script>
<style lang="scss" scoped>
header {
  display: flex;
  justify-content: center;
  padding: 50px 50px 0px;
  .left {
    flex: 1;
    .logo {
      width: 75px;
    }
  }
  .center {
    h3 {
      font-size: 32px;
      font-style: italic;
      font-weight: 400;
      margin: 0;
      &.buttom {
        text-align: right;
      }
    }
    h1 {
      color: #171717;
      font-size: 72px;
      margin: 0;
    }
  }
  .right {
    flex: 1;
    display: flex;
    justify-content: flex-end;

    label {
      position: relative;
      display: block;
      width: 300px;

      input {
        width: 100%;
        height: 35px;

        background-color: #ffffff;
        box-shadow: 2px 2px 8px 0px rgba(0, 0, 0, 0.2);

        margin: 0;
        padding: 5px 0px 0px 35px;
        box-sizing: border-box;

        appearance: none;
        border: none;
        outline: none;

        color: #171717;
        font-family: "Rockwell", serif;
        font-size: 16px;

        &::placeholder {
          color: #888888;
        }
      }
    }
    .icon {
      position: absolute;
      width: 25px;
      margin: 5px;
    }
  }
}
</style>
