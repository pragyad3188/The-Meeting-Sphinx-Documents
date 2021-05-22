---
title: Feasibility Study
layout: default
filename: pp
---
|[Home Page](index)| [Project Proposal](pp) | [Feasibility Study](fs) | [Design Document](design-doc) |
|--|--|--|--|

# Our Proposal

The essence of the software that we aim to build is an application that
runs in the background during meetings which detects when an attendee
starts to record the screen.

## The Problem

To understand the motivation behind us building a screen capture
detector, imagine the following scenarios:

-   A confidential meeting between a team of people who are discussing
    an important matter. This meeting cannot happen in person because of
    the lockdown, and no trace of the meeting should be left after it is
    over. Obviously, the meeting should not be recorded. It would be a
    problem if an attendee records the screen of his device using the
    inbuilt functionalities provided by its operating system. This gives
    rise to a need to stop screen recording, or at least detect it.

-   Another less critical, but more common incident is online class.
    Lazy and demotivated students do not pay attention in class,
    instead, they record the meeting so they can watch it later. Without
    active participation from the students, the class is less
    interactive, and provides a poor quality of education. If there was
    no way to record the screen, then the student has no choice but to
    attend class and pay attention. This, again, calls for a software to
    detect screen capture.

## What our software will do

In order to solve the problem described above, our software essentially
detects screen capture by any attendee, and informs the organizer of the
meeting. The following steps would be taken to use our software:

-   The organizer of the meeting creates a 'room' in our software which
    the attendees will join.

-   Each of the attendees will need to have installed our software on
    their device. Our software runs on the attendees' devices throughout
    the meeting, and as soon as it detects the sub-process that runs
    when the screen is recorded, it notifies the organizer of the
    meeting.

-   The organizer can see the list of attendees. The screen capture
    notification shows up next to the name of the attendee that starts
    recording.

-   As we can deduce, the organizer will not know if the attendee is
    recording the screen if the software is not installed on the
    attendee's device.

-   Hence, to ensure zero screen capture, we can suggest (enforce) the
    teacher (organizer of meeting) to take attendance through this
    software so that the students (attendees) MUST have this software
    installed and running.

## Why this is a good project for a team of 6 developers

There are many aspects to this project:

-   We need to understand operating systems to know which sub-processes
    run when a screen is being recorded.

-   We need an application running on the device of each attendee and
    meeting organizer.

-   We must also create a server application that coordinates between
    the members of the meeting and creates the room.

-   We must also design and develop a front-end user interface for the
    meeting organizer to see the attendees.

The above tasks can be divided among the members of our team, and we aim
to comfortably finish building the software within the given time frame.
