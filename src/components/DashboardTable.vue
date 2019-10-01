<template>
  <div class="dashboard__table">
    <div class="dashboard__inputs">
        <!-- <div class="input__select"> -->
          <select name="role" id="role" class="input__select">
            <option value="Your role">Your roles</option>
          </select>
        <!-- </div> -->
      <MyButton>Change</MyButton>
      <input placeholder="Enter Staff name here" type="text" class="input__text">
    </div>
    <table>
      <tr>
        <th class="table__heading">
          <input type="checkbox" name="" id="">
        </th>
        <th>First Name</th>
        <th>Last Name</th>
        <th>email</th>
        <th>Phone Number</th>
        <th>Role</th>
        <th></th>
      </tr>
      <tableRow />
      <tableRow />
      <tableRow />
      <tableRow />
    </table>
  </div>
</template>

<script>
import TableRow from "../components/TableRow";
import MyButton from "../components/Button";
export default {
  components: {
    MyButton,
    TableRow
  }
}
</script>

<style lang="scss">
  .input{
    
    &__select, &__text {
      border: 1px solid rgba(106, 126, 138, 0.4);
      background: white;
      border-radius: 3px;
      padding: 1rem;
      margin-right: 1rem;
    }

    &__select {
      margin-right: 1rem;      
    }


    &__text {
      margin-left: 1rem;
    }
  }

  table {
    margin-top: 1rem;
    width: 100%;
    border-collapse: separate;
    border-spacing: 0 1rem;

    tr {
      padding: 1rem 0;
      border-radius: 3px;
    }

    th {
      color: #013C61;
      text-transform: capitalize;
      text-align: left;
    }

    td, th {
      border: none;
      padding-top:20px;
      padding-bottom:20px;
      padding-right:20px;   
    }

    td:first-child, th:first-child {
      padding-left:20px;
      padding-right:0;
    }

    .table__body {
      background-color: white;
    }

    td { border: solid 1px #fff; }
    tr td:first-child {
       border-top-left-radius: 10px;
       border-bottom-left-radius: 10px; 
    }
    tr td:last-child { 
      border-top-right-radius: 10px; 
    }
    tr td:first-child { border-bottom-left-radius: 10px; }
    tr td:last-child { border-bottom-right-radius: 10px; }
  }
</style>