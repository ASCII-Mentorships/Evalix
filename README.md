# Evalix

## Introduction

Evalix is an application for simplifying and automating the evaluation steps for coding labs in BITS Goa.

## Goal

- The end goal of this project is to provide a free & locally hosted alternative to paid platforms like HackerRank for conducting evaluative lab components.
- To ultimately reduce the need for TAs manually evaluating each student’s code within the lab.
- To allow students to execute their code with standard or custom testcases in realtime.

## Description & Target Functionality

The overall project will involve the development of two applications. One will be for the administrator/instructor - referred to as the **Admin App**, and the other will be for the student - referred to as the **Student App**.

### Admin App

This will involve a simple server running on a docker image. For every lab component, the instructor will be required to set-up the following options -

- [ ] Programming Language
- [ ] Expected files in Submission
- [ ] Visible Test Cases
- [ ] Hidden Test Cases
- [ ] Marking Scheme

This initial setup will be done through a React app.

Once the setup is complete, the instructor can start hosting the submission server. This will make the assignment live and hence visible to instances of Student App running on the shared local network.

Whenever a student is satisfied with their submission, they’ll upload the required file/s on the Student App, which will send it over to the Admin App for saving. The Admin App will also expose some visible test cases to the students, which the students can execute locally (from the Student App) to test the supposed accuracy of their submission. These test-cases made visible to the students can be edited by the instructor live, so if any problematic test-case is reported during the lab, the error can be rectified in real-time.

After the submission window has concluded, the admin will have access to all the student submissions and data associated with it. They will have the option to modify the test-cases, and re-run them on all the submissions, and generate a CSV with the scores.

### Student App

This app will also be an independent node server app running on a docker image within every student’s computer. Security measures will be implemented to prevent computers from outside the lab imitating a computer from within the lab.

This app will host a React client for the student to run their code locally and to make submissions from. Once a student is sufficiently satisfied with their attempt at solving the lab, they can drag and drop their submission file/s on the client, and either run the standard or custom test cases locally, or they can submit the file/s to the admin app for final grading.

There is a docker image at the base for running each of these apps, as the code execution will be done within the docker container itself.

## Plan of Action or Time Line

We plan to work for around 12-15 weeks. Note that the following is just a tentative course of action.

- Week 1: Introduction and detailed understanding of the Project.
- Weeks 2-3: Learning and getting familiar with the Tech Stack and technologies.
- Weeks 4-5: Developing UI (making wireframe and the prototypes).
- Weeks 6-8: Development of the Admin App.
- Weeks 9-10: Development of the Student App.
- Weeks 10-12: Integration testing and bug-fixing.
- Week 13: Demo readiness.

## Technologies

- Docker
- Node
- React

## Prerequisites

- Basic coding experience.
- Basic understanding of web development.
- Appreciated optional stuff:
  - React
  - Node
  - Docker

## Project Mentors

- [Manthan Asher](https://github.com/Manthan-Asher)
- [Shameek Baranwal](https://github.com/shameekbaranwal)
- [Rajath V](https://github.com/Rajath-55)
- [Taarush Bhatia](https://github.com/Taarushthenoob)
- [Akhilesh Adithya](https://github.com/AkhileshAdithya)
