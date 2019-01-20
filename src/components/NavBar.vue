<template>
<b-navbar toggleable="md" type="dark" variant="dark">

  <b-navbar-toggle target="nav_collapse"></b-navbar-toggle>

  <b-navbar-brand to='/'>QC Web</b-navbar-brand>

  <b-collapse is-nav id="nav_collapse">

    <b-navbar-nav>
      <b-nav-item to='/screen1'>Screen1</b-nav-item>
      <b-nav-item to='/screen2'>Screen2</b-nav-item>
      <b-nav-item to='/screen3'>Screen3</b-nav-item>
      <b-nav-item to='/screen4'>Screen4</b-nav-item>
      <b-nav-item to='/screen5'>Screen5</b-nav-item>
      <b-nav-item to='/screen6'>Screen6</b-nav-item>
      <b-nav-item to='/screen7'>Screen7</b-nav-item>
    </b-navbar-nav>

    <!-- Right aligned nav items -->
    <b-navbar-nav class="ml-auto">

      <b-nav-form>
        <b-form-input size="sm" class="mr-sm-2" type="text" placeholder="Search"/>
        <b-button size="sm" class="my-2 my-sm-0" type="submit">Search</b-button>
      </b-nav-form>

      <b-nav-item-dropdown text="Lang" right>
        <b-dropdown-item href="#">EN</b-dropdown-item>
        <b-dropdown-item href="#">ES</b-dropdown-item>
        <b-dropdown-item href="#">RU</b-dropdown-item>
        <b-dropdown-item href="#">FA</b-dropdown-item>
      </b-nav-item-dropdown>

      <b-nav-item-dropdown right>
        <!-- Using button-content slot -->
        <template slot="button-content">
          <em>User</em>
        </template>
        <b-dropdown-item to='/login'>Sign In</b-dropdown-item>
        <b-dropdown-item href="#"> Fake Login</b-dropdown-item>
        <b-dropdown-item to='/logout'>Signout</b-dropdown-item>
      </b-nav-item-dropdown>
    </b-navbar-nav>

  </b-collapse>
</b-navbar>
</template>

<script>
</script>
