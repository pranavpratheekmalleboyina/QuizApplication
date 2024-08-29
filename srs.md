# Software Requirements Specification (SRS)

This SRS document outlines the necessary specifications for the online course authoring and teaching web application. It serves as a comprehensive guide for the development team to build a robust and user-friendly system.

Online Course Authoring and Teaching Web Application

## 1. Introduction

**1.1 Purpose**
This document specifies the requirements for an online course authoring and teaching web application that allows instructors to create and manage courses, including uploading pre-recorded videos and creating pre-written quizzes. Students will be able to access these courses, view the videos, take quizzes, and proceed to the next sections based on their quiz results.

**1.2 Scope**
The web application will include functionalities for course creation, video management, quiz management, user management, progress tracking, and reporting. It will cater to instructors and students, providing a seamless and interactive learning experience.

**1.3 Definitions, Acronyms, and Abbreviations**
<u>SRS:</u> Software Requirements Specification
<u>Admin:</u> Administrator of the system
<u>Instructor:</u> User who creates and manages courses
<u>Student:</u> User who takes courses

**1.4 References**
IEEE Std 830-1998, IEEE Recommended Practice for Software Requirements Specifications
<u>Online Course Platforms: </u>Coursera, Udemy, edX, <a>https://quiz.com/ </a>

**1.5 Overview**
This document contains detailed descriptions of the system's functionalities, interfaces, and constraints. It is organized into several sections, including system features, external interface requirements, system requirements, and other non-functional requirements.

##  2. Overall Description
**2.1 Product Perspective**
The application will be a standalone web-based system, accessible via standard web browsers. It will integrate with third-party video hosting services and payment gateways.

**2.2 Product Functions**
<u>Course Management:</u> Instructors can create, edit, and delete courses.
<u>Video Management:</u> Instructors can upload and manage pre-recorded videos.
<u>Quiz Management:</u> Instructors can create, edit, and delete quizzes.
<u>Media Management:</u> Instructors can include videos,images,memes,etc. as part of the quiz questions.
<u>Student Progress Tracking:</u> The system tracks student progress and quiz results.
<u>User Management:</u> Admins can manage user accounts and roles.
<u>Seamless Integration:</u> Users can sign in through the site or through email or social media handles.
<u>Competitiveness:</u> The students can view their results and a  real-time leaderboard instantly after the quizzes.
<u>AI compatibility:</u> Generating quizzes automatically based on a certain topic.
<u>Access Control:</u> The system controls access to course content based on quiz results.
                       Seamless access from all social media handles.

**2.3 User Classes and Characteristics**
<u>Admins:</u> Manage the overall system, user roles, and permissions.
<u>Instructors:</u> Create and manage courses, videos, and quizzes.
<u>Students: </u>Enroll in and take courses, view videos, and take quizzes.

**2.4 Operating Environment**
<u>Client Side: </u>Any modern web browser (Chrome, Firefox, Safari, Edge)
<u>Server Side: </u>Linux-based server with a web server (e.g., Apache or Nginx), a relational database (e.g., MySQL or PostgreSQL), and a backend framework (e.g., Django, Flask, or Node.js).

**2.5 Design and Implementation Constraints**
<u>Compliance with W3C standards:</u> The application must adhere to web standards.
<u>Security:</u> The system must ensure data protection and user privacy.

**2.6 User Documentation**
<u>User Manual:</u> Detailed guide for using the system.
<u>Online Help:</u> Context-sensitive help within the application.

**2.7 Assumptions and Dependencies**
Reliable internet connection for accessing the web application.
Third-party services for video hosting and payment processing are operational.

## 3. System Features
#### 3.1 Course Management
##### 3.1.1 Description and Priority
Instructors can create and manage courses. This is a high-priority feature.

##### 3.1.2 Functional Requirements

<u>FR1:</u> Instructors can create new courses.
<u>FR2: </u>Instructors can edit existing courses.
<u>FR3:</u> Instructors can delete courses.
<u>FR4:</u> Instructors can view a list of all their courses.
<u>FR5:</u> Instructors can see get a results in the form of a leaderboard.
#### 3.2 Video Management
##### 3.2.1 Description and Priority
Instructors can upload and manage pre-recorded videos. This is a high-priority feature.

##### 3.2.2 Functional Requirements

<u>FR1:</u> Instructors can upload videos.
<u>FR2:</u>Instructors can organize videos into course sections.
<u>FR3:</u> Instructors can delete videos.
<u>FR4:</u> Instructors can view a list of all uploaded videos.

#### 3.3 Quiz Management
##### 3.3.1 Description and Priority
Instructors can create and manage quizzes. This is a high-priority feature.

##### 3.3.2 Functional Requirements

<u>FR1:</u> Instructors can create quizzes with multiple choice, true/false, and short answer questions.
<u>FR2:</u> Instructors can edit existing quizzes.
<u>FR3:</u> Instructors can delete quizzes.
<u>FR4:</u> Instructors can set passing criteria for quizzes.
<u>FR5:</u>

#### 3.4 Student Progress Tracking
##### 3.4.1 Description and Priority
The system tracks student progress and quiz results. This is a high-priority feature.

##### 3.4.2 Functional Requirements

<u>FR1: </u>The system records student progress through course sections.
<u>FR2: </u>The system tracks quiz results.
<u>FR3: </u>The system allows students to view their progress and quiz results.
<u>FR4:</u>The system should allow students to upload their photo.
<u>FR5:</u>The system should allow the students to pause the quiz at any time.
#### 3.5 User Management
##### 3.5.1 Description and Priority
Admins can manage user accounts and roles. This is a medium-priority feature.

##### 3.5.2 Functional Requirements

<u>FR1: </u>Admins can create, edit, and delete user accounts.
<u>FR2: </u>Admins can assign roles to users (Admin, Instructor, Student).
<u>FR3: </u>Admins can view a list of all users.

#### 3.6 Access Control
##### 3.6.1 Description and Priority
The system controls access to course content based on quiz results. This is a high-priority feature.

##### 3.6.2 Functional Requirements

<u>FR1:</u> The system restricts access to subsequent course sections until a student passes the current section's quiz.
<u>FR2:</u> The system grants access to the next section upon passing the quiz.

## 4. External Interface Requirements

#### 4.1 User Interfaces
<u>UI1:</u> Course creation and management interface for instructors.
<u>UI2:</u> Video upload and management interface for instructors.
<u>UI3:</u> Quiz creation and management interface for instructors.
<u>UI4:</u> Course browsing and progress tracking interface for students.
<u>UI5:</u> Admin dashboard for managing users and roles.

#### 4.2 Hardware Interfaces
Not applicable.

#### 4.3 Software Interfaces
<u>SI1:</u> Integration with video hosting services (e.g., YouTube, Vimeo).
<u>SI2:</u> Integration with payment gateways (e.g., PayPal, Stripe).

##### 4.4 Communications Interfaces
<u>CI1:</u> HTTPS for secure communication between clients and the server.

## 5. System Requirements
#### 5.1 Functional Requirements
Covered in section 3.

#### 5.2 Non-Functional Requirements
##### 5.2.1 Performance Requirements

The system should support at least 1000 concurrent users.
The system should load pages within 2 seconds.

##### 5.2.2 Security Requirements

The system must protect user data with encryption.
The system must have secure authentication and authorization mechanisms.

##### 5.2.3 Usability Requirements

The system must be easy to navigate for all user roles.
The system must provide a responsive design for use on various devices.

##### 5.2.4 Reliability Requirements

The system should have an uptime of 99.9%.

##### 5.2.5 Maintainability Requirements

The system should have modular code for ease of maintenance.
The system should have comprehensive documentation for developers.

##### 5.2.6 Portability Requirements

The system should be deployable on various web servers.

## 6. Other Requirements
#### 6.1 Legal and Regulatory Requirements
The system must comply with data protection regulations (e.g., GDPR, CCPA).
The system must comply with accessibility standards (e.g., WCAG 2.1).
#### 6.2 Ethical Requirements
The system should ensure fair use and prevent academic dishonesty.

## 7. Appendices
#### 7.1 Glossary
<u>Course:</u> A set of instructional materials including videos and quizzes.

<u>Quiz:</u> A set of questions to assess student understanding.

<u>Section:</u> A subdivision of a course, typically containing a video and a quiz.





