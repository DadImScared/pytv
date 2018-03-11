
pytv for Python
===================

This library uses the `tvmaze <http://www.tvmaze.com/api>`_
API. All data is credited to them.

This
documentation
is a work
in progress


Installation:

    pip install pytv

Usage

    from pytv import Show, Schedule


    Get schedule for current day::

        >>>schedule = Schedule()
        >>>schedule.episodes
        [list of episodes]

    Get schedule for other days::

        >>>schedule = Schedule(date='2011-25-12')

    Get a show::

        >>>show = Show(show_id=1)
        >>>show.name
        'Under The Dome'

The Show class has the following attributes:

- episodes
- specials
- seasons
- cast
- crew
- next_episode
- summary
- name
- premiered

Search class:

    init: variant, query, lookup

    query: required if variant is in [show, singlesearch, people]

    lookup: required if variant is lookup

    variant options:

    - show(default)
    - singlesearch
    - lookup
    - people

    attributes:

    - results (list if variant in [show, people] single object if other)

Search usage

  from pytv import Search

  search shows::

    >>>search = Search(query='breaking bad')
    >>>search.results
    [list of results as Show objects]

  lookup tvdb id::

    >>>search = Search(variant="lookup", lookup="thetvdb=81189")
    >>>search.results
    (Show object)

