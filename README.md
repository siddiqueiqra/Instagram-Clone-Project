# Instagram Clone Project

## Overview

This project aims to create a simplified version of Instagram, focusing on the database design using SQL. The goal is to replicate some of the key features of Instagram, such as user management, photo sharing, and interactions.

## Features

- **User Management:** Users can create accounts, log in, and update their profiles.
- **Photo Sharing:** Users can upload photos, add captions, and share them with their followers.
- **Followers/Following:** Users can follow and unfollow other users to build a network.
- **Feed:** A personalized feed for each user displaying posts from the users they follow.
- **Likes and Comments:** Users can like and comment on photos.

## Tech Stack

- **Database:** SQL (Structured Query Language)

## Database Schema

The database design will be crucial to the functionality of the application. Here's a simplified schema:

### Tables

1. **Users**
   - UserID (Primary Key)
   - Username
   - Email
   - Password
   - Profile Picture
   - ...

2. **Posts**
   - PostID (Primary Key)
   - UserID (Foreign Key to Users)
   - Image
   - Caption
   - LikesCount
   - ...

3. **Followers**
   - FollowerID (Primary Key)
   - FollowerUserID (Foreign Key to Users)
   - FollowingUserID (Foreign Key to Users)
   - ...

4. **Comments**
   - CommentID (Primary Key)
   - PostID (Foreign Key to Posts)
   - UserID (Foreign Key to Users)
   - Text
   - ...

