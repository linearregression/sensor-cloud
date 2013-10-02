Project Skeleton for the engine app.

You should find in this directory:

README : this file
Makefile : simple make commands
rebar : the Rebar build tool for Erlang applications
rebar.config : configuration for Rebar
start.sh : simple startup script for running engine
/ebin
  /engine.app : the Erlang app specification
/src
  /engine_app.erl : base module for the Erlang application
  /engine_sup.erl : OTP supervisor for the application
/priv
  /dispatch.conf : the Webmachine URL-dispatching table
  /www : a convenient place to put your static web content

You probably want to do one of a couple of things at this point:

0. Build the skeleton application:
   $ make
   - or -
   $ ./rebar compile

1. Start up the skeleton application:
   $ ./start.sh

2. Change the basic application:
   edit src/engine_resource.erl

3. Add some new resources:
   edit src/YOUR_NEW_RESOURCE.erl
   edit priv/dispatch.conf
