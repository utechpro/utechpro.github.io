<template>
  <div id="app">
    <div id="header">
      <div style="box-sizing: initial;position: fixed;top: 0; left: 0;background: white;width: 100%;padding: 15px;color: black;-webkit-box-shadow: 0px 0px 8px 2px rgba(0,0,0,.1);
       -moz-box-shadow: 0px 0px 8px 2px rgba(0,0,0,.1);z-index: 10000000;height: 40px;line-height: 40px;
            box-shadow: 0px 0px 8px 2px rgba(0,0,0,.1);">
        
        <div style="float: left;padding-left: 15px;">
    	    <img src="images/logo4.png" style="vertical-align: middle;" />
        </div>
        
        <div style="float: right;font-size: 1.1em;">
            <ul id="menu_items">
              <li>
                <i class="fa fa-wrench" aria-hidden="true"></i>
                <span>
                  <a id="projects_link" href="/dashboard">Наша история успеха</a>
                </span>
              </li>
              <li>
                <i class="fa fa-map-marker" aria-hidden="true"></i>
                <span>
                  <a id="projects_link" href="/dashboard">Как нас найти?</a>
                </span>
              </li>
              <li>
                <i class="fa fa-shopping-cart" aria-hidden="true"></i>
                <span>
                  <router-link to="/about">Личный кабинет</router-link>
                </span>
              </li>
              <li>
                <i class="fa fa-phone" aria-hidden="true"></i>
                <span>
                  <b style="line-height: 30px;font-weight: normal;">(3452) 38-72-11</b>
                </span>
              </li>
            </ul>
        </div>
        <div style="clear: both;"></div>
      </div>
    </div>
    <router-view/>
  </div>
</template>

<style>
#app {
  font-family: pfhighway,Helvetica,sans-serif;
  color: white;
  text-align: center;
}

#header {
  z-index: 999999999;
}

#menu_items a {
  line-height: 30px;
  font-weight: normal;
  text-decoration: none;
  color: black;
}

#menu_items {
  display: inline;
  list-style-type: none;
  font-size: 0.9em;
}

#menu_items li {
  display: inline;
  padding: 13px 0;
  margin-right: 30px;
  cursor: pointer;
  position: relative;
}

#menu_items li i {
  color: #09736b;
  margin-right: 7px;
  font-size: 1.4em;
  vertical-align:middle;
}

#menu_items li:hover {
}

#menu_items li span {
  position: relative;
}

#menu_items li:hover span:after {
  width: 40%;
  border-bottom: 3px solid #09736b;
  transform: translate(-50%);
  content: "";
  position: absolute;
  left: 50%;
  margin: 38px auto;
}
</style>