<template>
  <div class="head">
    <header>
      <div class="row">
        <div class="logo-container col">
          <img src="/images/avada-bakery-logo.png" alt="logo">
        </div>
        <nav class="col">
          <ul>
            <li>HOME</li>
            <li>HOME</li>
            <li>HOME</li>
          </ul>
        </nav>
      </div>
    </header>
    <div class="jumbo">

    </div>
  </div>
</template>

<script>
export default {
  
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

.head {
  background: url('/images/hero-header-bakery.jpg') 50% 50%;
  background-size: cover;
  height: 600px; // da sistemare

  header {
    height: 100px;
    padding: 10px 20px;

    .row {
      height: 100%;

      .logo-container {
        height: 100%;
        img {
          height: 100%;
        };
      }

      nav {
        height: 100%;
        padding: 20px 10px;

        ul {
          height: 100%;
          list-style: none;
          color: $primary;
          display: flex;
          justify-content: flex-end;
          align-items: center;
          li {
            font-size: .8rem;
            margin-left: 30px;
            cursor: pointer;
            padding: 6px 0;
            &:hover {
              border-bottom: 2px solid $primary;
            }
          }
        }
      }
    }

  }
}
</style>