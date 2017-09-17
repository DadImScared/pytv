
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