README.md
=========

Commands used:
``` sh 
rails new testing && cd testing/
rails generate scaffold user
rake db:migrate 
rails server
```

$ rails s
=> Booting WEBrick
=> Rails 4.1.1 application starting in development on http://0.0.0.0:3000
=> Run `rails server -h` for more startup options
=> Notice: server is listening on all interfaces (0.0.0.0). Consider using 127.0.0.1 (--binding option)
=> Ctrl-C to shutdown server
[2014-06-23 10:01:22] INFO  WEBrick 1.3.1
[2014-06-23 10:01:22] INFO  ruby 2.1.2 (2014-05-08) [x86_64-darwin13.0]
[2014-06-23 10:01:22] INFO  WEBrick::HTTPServer#start: pid=2437 port=3000


Started GET "/" for 127.0.0.1 at 2014-06-23 10:01:27 -0700
ActiveRecord::SchemaMigration Load (0.1ms)  SELECT "schema_migrations".* FROM "schema_migrations"
Processing by Rails::WelcomeController#index as HTML
Rendered /Users/jason/.rbenv/versions/2.1.2/lib/ruby/gems/2.1.0/gems/railties-4.1.1/lib/rails/templates/rails/welcome/index.html.erb (1.5ms)
Completed 200 OK in 17ms (Views: 7.2ms | ActiveRecord: 0.0ms)


Started GET "/users" for 127.0.0.1 at 2014-06-23 10:01:27 -0700
Processing by UsersController#index as HTML
User Load (0.1ms)  SELECT "users".* FROM "users"
Rendered users/index.html.erb within layouts/application (1.3ms)
Completed 200 OK in 587ms (Views: 585.0ms | ActiveRecord: 0.1ms)


Started GET "/assets/users.css?body=1" for 127.0.0.1 at 2014-06-23 10:01:28 -0700


Started GET "/assets/scaffolds.css?body=1" for 127.0.0.1 at 2014-06-23 10:01:28 -0700


Started GET "/assets/jquery_ujs.js?body=1" for 127.0.0.1 at 2014-06-23 10:01:28 -0700


Started GET "/assets/application.css?body=1" for 127.0.0.1 at 2014-06-23 10:01:28 -0700


Started GET "/assets/jquery.js?body=1" for 127.0.0.1 at 2014-06-23 10:01:28 -0700


Started GET "/assets/turbolinks.js?body=1" for 127.0.0.1 at 2014-06-23 10:01:28 -0700


Started GET "/assets/users.js?body=1" for 127.0.0.1 at 2014-06-23 10:01:28 -0700


Started GET "/assets/application.js?body=1" for 127.0.0.1 at 2014-06-23 10:01:28 -0700


Started GET "/usr" for 127.0.0.1 at 2014-06-23 10:01:30 -0700

Started GET "/users/" for 127.0.0.1 at 2014-06-23 10:01:33 -0700
Processing by UsersController#index as HTML
User Load (0.2ms)  SELECT "users".* FROM "users"
Rendered users/index.html.erb within layouts/application (0.9ms)
Completed 200 OK in 6ms (Views: 5.7ms | ActiveRecord: 0.2ms)


Started GET "/assets/users.css?body=1" for 127.0.0.1 at 2014-06-23 10:01:33 -0700


Started GET "/assets/application.css?body=1" for 127.0.0.1 at 2014-06-23 10:01:33 -0700


Started GET "/assets/turbolinks.js?body=1" for 127.0.0.1 at 2014-06-23 10:01:33 -0700


Started GET "/assets/jquery.js?body=1" for 127.0.0.1 at 2014-06-23 10:01:33 -0700


Started GET "/assets/application.js?body=1" for 127.0.0.1 at 2014-06-23 10:01:33 -0700


Started GET "/assets/scaffolds.css?body=1" for 127.0.0.1 at 2014-06-23 10:01:33 -0700


Started GET "/assets/users.js?body=1" for 127.0.0.1 at 2014-06-23 10:01:33 -0700


Started GET "/assets/jquery_ujs.js?body=1" for 127.0.0.1 at 2014-06-23 10:01:33 -0700


Started GET "/users/new" for 127.0.0.1 at 2014-06-23 10:01:34 -0700
Processing by UsersController#new as HTML
Rendered users/_form.html.erb (9.7ms)
Rendered users/new.html.erb within layouts/application (11.1ms)
Completed 200 OK in 17ms (Views: 15.9ms | ActiveRecord: 0.3ms)


Started GET "/" for 127.0.0.1 at 2014-06-23 10:01:35 -0700
Processing by Rails::WelcomeController#index as HTML
Rendered /Users/jason/.rbenv/versions/2.1.2/lib/ruby/gems/2.1.0/gems/railties-4.1.1/lib/rails/templates/rails/welcome/index.html.erb (0.1ms)
Completed 200 OK in 1ms (Views: 1.0ms | ActiveRecord: 0.0ms)


Started POST "/users/new" for 127.0.0.1 at 2014-06-23 10:01:35 -0700

ActionController::RoutingError (No route matches [POST] "/users/new"):
actionpack (4.1.1) lib/action_dispatch/middleware/debug_exceptions.rb:21:in `call'
actionpack (4.1.1) lib/action_dispatch/middleware/show_exceptions.rb:30:in `call'
railties (4.1.1) lib/rails/rack/logger.rb:38:in `call_app'
railties (4.1.1) lib/rails/rack/logger.rb:20:in `block in call'
activesupport (4.1.1) lib/active_support/tagged_logging.rb:68:in `block in tagged'
activesupport (4.1.1) lib/active_support/tagged_logging.rb:26:in `tagged'
activesupport (4.1.1) lib/active_support/tagged_logging.rb:68:in `tagged'
railties (4.1.1) lib/rails/rack/logger.rb:20:in `call'
actionpack (4.1.1) lib/action_dispatch/middleware/request_id.rb:21:in `call'
rack (1.5.2) lib/rack/methodoverride.rb:21:in `call'
rack (1.5.2) lib/rack/runtime.rb:17:in `call'
activesupport (4.1.1) lib/active_support/cache/strategy/local_cache_middleware.rb:26:in `call'
rack (1.5.2) lib/rack/lock.rb:17:in `call'
actionpack (4.1.1) lib/action_dispatch/middleware/static.rb:64:in `call'
rack (1.5.2) lib/rack/sendfile.rb:112:in `call'
railties (4.1.1) lib/rails/engine.rb:514:in `call'
railties (4.1.1) lib/rails/application.rb:144:in `call'
rack (1.5.2) lib/rack/lock.rb:17:in `call'
rack (1.5.2) lib/rack/content_length.rb:14:in `call'
rack (1.5.2) lib/rack/handler/webrick.rb:60:in `service'
/Users/jason/.rbenv/versions/2.1.2/lib/ruby/2.1.0/webrick/httpserver.rb:138:in `service'
/Users/jason/.rbenv/versions/2.1.2/lib/ruby/2.1.0/webrick/httpserver.rb:94:in `run'
/Users/jason/.rbenv/versions/2.1.2/lib/ruby/2.1.0/webrick/server.rb:295:in `block in start_thread'


Rendered /Users/jason/.rbenv/versions/2.1.2/lib/ruby/gems/2.1.0/gems/actionpack-4.1.1/lib/action_dispatch/middleware/templates/rescues/_trace.html.erb (1.0ms)
Rendered /Users/jason/.rbenv/versions/2.1.2/lib/ruby/gems/2.1.0/gems/actionpack-4.1.1/lib/action_dispatch/middleware/templates/routes/_route.html.erb (1.3ms)
Rendered /Users/jason/.rbenv/versions/2.1.2/lib/ruby/gems/2.1.0/gems/actionpack-4.1.1/lib/action_dispatch/middleware/templates/routes/_table.html.erb (1.0ms)
Rendered /Users/jason/.rbenv/versions/2.1.2/lib/ruby/gems/2.1.0/gems/actionpack-4.1.1/lib/action_dispatch/middleware/templates/rescues/routing_error.html.erb within rescues/layout (19.8ms)

