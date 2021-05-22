---
title: Feasibility Study
layout: default
filename: fs
---
| [Home Page](index) | [Project Proposal](pp) | [Feasibility Study](fs) | [Design Document](design-doc) |


# Customer

Our customer base would include any person who wants to conduct a
meeting or a class online in a secure manner. As people sometimes say
things informally which they don't want to be recorded, an app that
would notify them whenever someone starts recording would be a perfect
solution, as they can speak consciously from then onward.

## Why not an app that completely stops the recording instead?

We first tried to research on making an app that could completely stop
the recording of meetings, but it was rendered infeasible as it would
require admin privileges of the attendee's system. And it might raise
privacy issues from the attendee's side.

# Visibility Study

We plan to keep contact with the customer on a weekly basis:

-   Schedule an online meeting with the customer and provide real time
    updates in a one to one interactive session.

-   Provide a broad overview of a feasible timeline for the project and
    discuss their queries.

-   Provide a written **Progress Report** of all the additional features
    or changes over the past week.

We plan to have a smooth communication between the team members through:

-   Daily meetups regarding the amount of assigned work done.

-   Project Collaboration through effective version control software
    like git.

-   An active discussion forum on collaborative platforms like slack
    where any queries regarding the project design and errors can be
    discussed across all the team members.

# Task to be Undertaken

Develop an application for an organiser to schedule meetings with
several attendees.

-   Video conferencing would be present

-   The people in the meeting would also be able to chat using the
    inbuilt chat feature.

-   The app would notify the organiser whenever an attendee starts to
    record the screen. It achieves this by running a program in the
    background.

Develop a software that meeting organisers can use as a third party
application so as to detect screen recording while organising meetings
in other platforms.

-   The organisers would use this as an app for taking attendance (This
    is specially meant for online classes). The organiser makes it
    compulsory for the attendees of the meeting to have this app
    installed and running.

-   This app would detect the recording of the meeting by an attendee
    and would notify the organiser of the class.

# Preliminary Requirement Analysis

The first major requirement of our project is to make a detection
software. For this we had to analyse the various screen recording
softwares that are in use currently. We studied the various processes
that run in the background when a screen recorder is recording the
screen. We mapped the screen recorders to the system processes that they
use when screen recording is being done. These processes were listed and
our detection algorithm plans to detect these processes running in the
background.

The next concern of our project was how to make this software in use. We
are making a platform itself so as to conduct meetings and online
classes, in which our recording software would run in the background and
notify the organiser when someone starts recording.

Some people would not like to switch platforms from the current platform
in which they are conducting their class. To tackle this, we have our
second version of our software which can be used as a third-party
application to take attendance, which would notify the meeting organiser
about any screen recording being done.

# Suggested Deliverables

We plan to deliver two different applications by the end of our project:
A native linux application for tracking if the user is recording his /
her screen and a platform which implements the command line application
and provides a video conferencing functionality to the users. Our course
of action can be found in the section **Outlined Plan** (below).
Adhering to the agile model, we will be delivering a number of partially
complete, but working applications during the course of our project.
Some of the deliverables in the order that they would be delivered are
as follows:

-   **CLI** A basic program that would detect if the user starts a
    screen recorder. Using this, we can show the user that our app is
    working.

-   **Frontend Backend** Basic WebRTC implementation over the
    frontend and integration with backend.

-   **CLI** The complete CLI that would be capable of docking the
    frontend build over it.

-   **Coupling** Refactoring of the codebase and writing code for
    coupling of the frontend, the CLI and the backend.

-   **Deployment** Make the final deployment build of the
    sub-projects.

# Process to be followed

We plan to work using the Agile methodology. In specific:

-   Deliver working code in every week's tutorial.

-   Have daily meetings to either work on the code or discuss design
    plans.

-   In every GBM, reflect on how we performed in that week and discuss
    on how we can improve in the coming week.

-   We plan on coding following the principles of pair programming like
    the code review principle. While one person writes the code, the
    other member would verify its correctness and also give appropriate
    feedback, and this role would alter with every run.

We plan to use Extreme Programming in the following way:

-   Write Django tests to regularly check if addition of any new
    features interfered with the old code, to perform integration
    testing.

-   Write simple yet efficient code with the most recent and updated
    frameworks.

-   Have daily meetings to either work on the code or discuss design
    plans.

-   If at any point we feel that the code can be condensed or improved,
    we refactor it.

# Outline Plan

The following milestones would be achieved by us in order, so as to meet
the completion of our project :

-   First we would make a workflow of our app specifying the design and
    features and present it to the customer. Based on the feedback, we
    would make the required changes. This deadline is met already.

-   After the plan is finalised, the coding phase of our project begins.
    We would start by deciding the endpoints to make the required API
    calls in the frontend and backend both. This is essential as the
    views can be made only after finalising the endpoints. This phase is
    ongoing and is expected to be complete by 14/04/2021.

-   Then we make the program to detect the screen recording processes.
    This requires a lot of research as we have to investigate which all
    processes run for various screen recording applications. This is
    expected to be complete by 18/04/2021.

-   The views and models would be made in the backend and the required
    APIs would be implemented. This includes implementing a Video
    Conferencing platform using WebRTC, a chat platform using Django
    Channels, the notification of the screen record detection and a lot
    more minor features concerning our app. These features would be
    implemented using Django as the backend framework and React for the
    frontend. The expected time for completion of these is decided as
    30/04/2021.

-   The frontend build would be independent of the platform on which it
    will run. In parallel to the WebRTC implementation, a sub-team would
    be working on the CLI to convert it to a linux native app and write
    code for docking the frontend over the CLI in order to make our
    video conferencing platform. This CLI is expected to complete with
    the frontend build on 30/04/2021.

-   After the codebases of the frontend, backend and the detection
    algorithm have been set up separately, we need to integrate these
    into one software and resolve the issues that arise along with. We
    expect to complete this by 03/05/2021.

Thus, we can see from the outline, that our project is feasible within
the expected deadlines and using the good coding practices we would try
to meet the deadlines in a highly efficient manner.

# Risk Analysis

Our software could fail in the following scenarios:

-   A new screen recorder is released in the market that uses some
    process that our current software doesn't detect.

    -   We have planned to make the detection software in such a manner
        that only addition in such a case would be the name of the new
        process used by the new screen recorder. We would regularly
        check for new screen recording processes and keep on updating
        our software.

-   Probable risks in the integration of our detection software with our
    backend of meeting app.

    -   We have thought this of and realised that the detection program
        can be made using a different language in case the integration
        fails while using the current programming language. All major
        programming languages have libraries for dealing with system
        processes which can be made use of to meet the same requirement.

-   Customer doesn't like our app to conduct classes.

    -   We have made a second version of our app which can be used as a
        third party app for taking attendance. The customer can take
        meetings in their own platform and use this version of our app
        as a method for taking attendance. This would notify the class
        organiser of any background screen recording by any of the
        attendees.

# Probable Technical Requirements

As mentioned in the sections above, our project is classified into 3
different sub-projects. The probable technical requirements for each of
the sub-projects are as follows:

-   **CLI**

    -   We will be using a javascript framework for making a Linux
        native app.

    -   Then, we will use a framework like electron to deploy web apps
        on Linux native applications.

    -   After this, we will build a frontend to deploy on our Linux
        native app. We will be using a web development framework like
        ReactJS for achieving this.

    -   Since we know most of this tech stack, the implementation seems
        feasible.

-   **Frontend**

    -   We will be using a web development framework like React.

    -   Axios library will be used to handle requests made to and from
        the clients.

    -   A CSS library like SemanticUI will be used for making the
        frontend.

-   **Backend**

    -   We will be building our backend using a python backend framework
        like django.

    -   We will be using REST APIs and implementing web sockets for
        WebRTC.

    -   We will be using a database server like PostgreSQL for storing
        data and a message broker for implementing web sockets like
        redis.

    -   For deployment, we will be using dockerized images of our
        backend, message broker and our database.

    -   They will be deployed using docker-compose.
