
<div class="navbar navbar-fixed-top">
  <div class="navbar-inner">
    <div class="container">
 
      <!-- .btn-navbar is used as the toggle for collapsed navbar content -->
      <a class="btn btn-navbar" data-toggle="collapse" data-target=".nav-collapse">
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
      </a>
 
      <!-- Be sure to leave the brand out there if you want it shown -->
      <%= link_to "TRYSTO", root_path, class: "brand" %>
 
      <!-- Everything you want hidden at 940px or less, place within here -->
      <div class="nav-collapse collapse">
      	<ul class="nav">
        	<li><%= link_to "Home", root_path %></li>
					<li><%= link_to "About", about_path %></li>
				</ul>
				<ul class="nav pull-right">
        	<% if user_signed_in? %>
            <li><%= link_to "Edit Profile", edit_user_registration_path %></li>
            <li><%= link_to "Logout", destroy_user_session_path, method: :delete %></li>
          <% else %>
            <li><%= link_to "Login", new_user_session_path %></li>
          <% end %>
				</ul>
      </div>
 
    </div>
  </div>
</div>



# One Month Rails

This is the sample application for 
[*One Month Rails: Teach Yourself to Code*](http://onemonthrails.com)

by [Mattan Griffel](http://mattangriffel.com)