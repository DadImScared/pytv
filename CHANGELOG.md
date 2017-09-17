
# Pytv ChangeLog
____


## v0.2.0 (2017-09-16)
___

## New Classes:

* Episode
* Cast
* Crew

### Added:
* Schedule.episodes and Show.episodes now return a list of episodes as Episode objects
* Show.next_episode returns Episode object of the next episode to air
* Show.get_episode(int_here) returns Episode object based on number passed in or none if out of range


#### Fixed:

* Schedule().episodes properly errors if it's a bad date
