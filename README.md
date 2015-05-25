# Run-Program-Automatically-on-Startup
Run Program Automatically on Startup Under Ubuntu

# copy temlate to execution path
sudo cp template /etc/init.d/

# change mode for that file to execute things
sudo chmod +x /etc/init.d/template

# update template to work on start up
sudo update-rc.d /etc/init.d/template defaults

#commands to use after startup

#to start application
/etc/init.d/run_rails_app start

#to stop application
/etc/init.d/run_rails_app stop

#to restart application
/etc/init.d/run_rails_app restart

#to status application
/etc/init.d/run_rails_app status
