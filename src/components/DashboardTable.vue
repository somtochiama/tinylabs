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
    tr {
      padding: 1rem 0;
    }

    th {
      color: #013C61;
      text-transform: capitalize;
      text-align: left;
    }

    td {
      padding-top:20px;
      padding-bottom:20px;
      padding-right:20px;   
    }

    td:first-child {
      padding-left:20px;
      padding-right:0;
    }

    &__body {
      background-color: white;
    }

  }
</style>