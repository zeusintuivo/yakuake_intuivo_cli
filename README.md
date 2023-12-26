# yakuake_intuivo_cli

Do you use yakuake?
https://wiki.archlinux.org/title/Yakuake
https://wiki.archlinux.org/title/Yakuake

How to manage or open several sessions is a serious challenge

Here is a script to help do this 

Just create a file with a list of sessions

    touch my_sessions

    echo "
    vertical|sidekiq|/home/work/username/projects/sidekiqx
    simple|db|/home/work/username/projects/data|ls|split|/home/work/username/projects/db|ls|
    quad|tests|/home/work/username/projects/test|ls|bottom|/home/work/username/projects|ls|
    simple|push|/home/work/username/projects/project|git status|lest|/home/work/username/projects/project|git pull|
    horizontal|project|/home/work/username/projects/project|
    " > my_sessions

Here above 
 sessions type |name tab   |    folder                           | optional command to run  | split left or bottom optional | folder to open all new splits optional| optional command to run|         
 vertical      |sidekiq    |/home/work/username/projects/sidekiq |  ls                      |  left                         | /home/work/username/projects/sidekiq  | ls |
 quad
 horizontal
 simple
 flat


To run debug 
./yakuake_sessions --debug -2

To run
./yakuake_sessions my_sessions



you can create diverse files for diverse session configurations


