
# Pytv ChangeLog
___

## v0.3.0 (2018-03-10)

#### Fixed:
* proper error on 404

### Added:
* Search class
* Shows class
* get_updates

## v0.2.1 (2017-10-03)

#### Fixed:

* Show.cast properly returns list of cast members as Cast objects when initialized Show with embed_url with cast
* Show.crew properly returns list oc crew members as Crew objects when initialized Show with embed_url with crew

## v0.2.0 (2017-09-16)

### New Classes:

* Episode
* Cast
* Crew

### Added:
* Schedule.episodes and Show.episodes now return a list of episodes as Episode objects
* Show.next_episode returns Episode object of the next episode to air
* Show.get_episode(int_here) returns Episode object based on number passed in or none if out of range


#### Fixed:

* Schedule().episodes properly errors if it's a bad date
