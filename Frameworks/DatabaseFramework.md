# Database Architectural Decisions

- [Summary](#summary)
- [Issue](#issue)
- [Decision](#decision)
- [Status](#status)
- [Details](#details)
  - [Assumptions](#assumptions)
  - [Constraints](#constraints)
  - [Positions](#positions)
  - [Argument](#argument)
  - [Implications](#implications)
- [Related](#related)
  - [Related decisions](#related-decisions)
  - [Related requirements](#related-requirements)
  - [Related artifacts](#related-artifacts)
  - [Related principles](#related-principles)
- [Notes](#notes)

## Summary

### Issue

We need a backend database for saving user profiles and restaurants

- We want a easy to use and understandable database
- we want thew database to be flexible
- we want the database to have support and documentation

### Decision

Decided on MongoDB

### Status

Decided on MongoDB for our database systems. Open to other database frameworks should a NoSQL approach become unfeasable.

## Details

### Assumption

We want to choose a database framework that is scalable and flexible to support our development

- The development process will need to very fluid as problems are likely to come up as we encounter newbie problems

- We will need a database framework that is highly documented and trusted as well as cheap to maintain to make the development of the app easier

- MongoDB is known to be newbie friendly, which will make development easier.

we are using a NoSQL Database is beneficial for these reasons

### Constraints

If we start building a database with NoSQL and decide we would rather use SQL a transition would be difficult.

Relational data may also be better represented on a database such as oracle DB.

### Positions

We considered using Oracle as this is what we have the most experience in

We considered Maranda DB as this uses similar styling to what we have used before

Both are considered if a change is required

### Argument

as above others were not chosen due to the superior scalability and ease of use of MongoDB. We also want to explore more options outside of OracleDB for our own personal growth.

### Implications

We want something that is easily scalable and easy to use, we are flexible but would like to reduce any chance of a possible database overhaul.

## Related

### Related decisions

we want something that has lots of support

we don't want to have to search for obscure documentation

we all would like to learn a NoSQL database framework

### Related artifacts

This affects all calls made by our backend

### Related principles

trusted database

ease of use
