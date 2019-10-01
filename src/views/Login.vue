<template>
  <div class="login">
    <div class="login__img">
      <h3>No hazzle</h3>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
    </div>
    <div class="login__side">
      <div class="login__form">
        <h3>Create your free account</h3>
        <p>Already registered? <a href="#">Sign in.</a></p>
        <form action="">
          <div class="input__share">
            <div class="input__group half">
              <label for="firstName">First Name</label>
              <input type="text" name="firstName" id="">
            </div>
            <div class="input__group half">
              <label for="lastName">Last Name</label>
              <input type="text" name="lastName" id="">
            </div>
          </div>
          <div class="input__group">
            <label for="email">Email</label>
            <input type="email" name="email" id="">
          </div>
          <div class="input__group">
            <label for="password">Password</label>
            <input type="password" name="password" id="">
          </div>
          <MyBtn id="login-btn">Continue</MyBtn>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
import MyBtn from "../components/Button"
export default {
  components: {
    MyBtn
  }
}
</script>

<style lang="scss">
  .login {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    height: 100vh;

    &__img {
      background-image: url("../assets/model.png");
      background-repeat: no-repeat;
      background-size: cover;
      color: white;
      text-align: center;
      padding: 2rem 4rem;
      display: flex;
      flex-direction: column;
      justify-content: flex-end;
    }

    &__side {
      background-color: #FFFFFF;
      margin: 10rem;

      h3 {
        font-weight: 500;
        font-size: 34px;
        line-height: 46px;
      }

      p {
        font-size: 18px;
        a {
          text-decoration: none;
          color: #2BDA53;
        }
      }

      form {
        margin-top: 2rem;
        padding: 2rem 3rem 4rem;
        background: #FFFFFF;
        box-shadow: 0px 20px 50px #EAEEE9;
        border-radius: 5px;

        #login-btn {
          display: block;
            margin: 2rem 0 0 auto;
        }
        
        :first-child {
          margin-right: 1rem;
        }

        label {
          color: #6A7E8A;
        }

        input {
          padding: 1rem;
          border: none;
          border-bottom: 2px solid #E6E7EB;
          outline: none;
          display: block;
          width: 100%
        }

        .input__group {
          margin-top: 2rem;
        }

        .input__share {
          display: flex;
  
        }
  
        .input__group.half {
          width: 50%;
        }
      }

    }
  }


  @media screen and (max-width: 1000px) {
      .login {
      grid-template-columns: 40rem 1fr;
    }
  }

  @media screen and (max-width: 800px) {
      .login {
      grid-template-columns: 1fr;
      .login__img {
        display: none;
      }
    }
  }

  @media screen and (max-width: 500px) {
      .login {
      grid-template-columns: 1fr;

      &__img {
        display: none;
      }

      &__side{
        margin: 2rem;
        padding: 1rem 1.5rem 2rem;

        h3 {

        }

        p {

        }

        form {

          .input__share {
            flex-direction: column;
          }

          .input__group.half {
            width: 100%
          }

          .login-btn {
            width: 100%
          }
        }
      }

      .input__group.half {
        width: 100%;
      }
    }
  }
</style>