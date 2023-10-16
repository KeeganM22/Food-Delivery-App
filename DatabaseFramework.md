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

Decided on MongoDB open to a switch if called for

## Details

### Assumption

We want to choose a database that is very scalable and flexible to support our development 

We want something that is highly documented and trusted as well as cheap to maintain to support the future of our app 

using a NoSQL Database is beneficial for those reasons 

### Constraints

If we start building a database with NoSQL and decide we would rather use SQL a transition would be difficult

### Positions

We considered using Oracle as this is what we have the most experience in 

We considered Maranda DB as this uses similar styling to what we have used before 

Both are considered if a change is required 

### Argument

as above others were not chosen due to the superior scalability and want to explore more options 

### Implications

We want something that is easily scalable and easy to use, we are flexible but would like to reduce any chance of a possible database migration 

## Related

### Related decisions

we want something that has lots of support 

we don't want to have to search for obscure documentation 

### Related artifacts

this is the core of all of our information

### Related principles

trusted database

easy to use





