<template>

  <div class='demo1'>
    <navbar/>
      <form action="submit">
          <label for='firstname'>First Name : </label>
          <input type="text" id="firstname" placeholder="enter fisrt name"><br><br>

          <label for='lastname'>Last Name : </label>
          <input type="text" id="lastname" placeholder="enter last name"><br><br>

          <span>Gender : </span>
          <input type="radio" name="Gender" id="gender">
          <label for="gender">Male</label>
          <input type="radio" name="Gender" id="gender">
          <label for="gender">Female</label>
          <br>
          <br>

          <label for='number'>Mobile Number : </label>
          <input type="number" id="number" placeholder="Mobile Number"><br><br>

          <label for="addr">Address : </label>
          <textarea name="addr" id="addr" cols="30" rows="5"></textarea><br><br>

          <label for="city">City : </label>
          <select name="city" id="city">
              <option disabled value="">Select the city</option>
              <option value="nm">Navi Mumbai</option>
              <option value="mum">Mumbai</option>
              <option value="th">Thane</option>
          </select>
        <br>
        <br>
        <label for="state">State : </label>
          <select name="state" id="state">
              <option disabled value="">Select the state</option>
              <option value="mh">Mharashtra</option>
              <option value="rj">Rajasthan</option>
              <option value="goa">Goa</option>
          </select>
      </form>
    <br>
    <br>
    <button type="submit">Submit</button>
    <button type="reset">Reset</button>
    <footer/>
  </div>

</template>

<script>
import navbar from '../components/navbar.vue'
import footer from '../components/footer.vue'

export default {
  components:{
    navbar,
    footer,
  }


}
</script>

<style>
.demo1{
    
    background-color:aqua;
    margin:2px 2px 2px 2px;
    text-align: start;
    align-content: center;
}
</style>