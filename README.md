"# ATM-System" 
DATABASE :


create database bankSystem;
use bankSystem;

create table signup(form_no varchar(30), name varchar(30), father_name varchar(30), DOB varchar(30),gender varchar (30), email varchar(60) ,marital_status varchar(30),address varchar(60),city varchar(60),pincode varchar(60),state varchar(60));

select * from signup;

create table signuptwo(form_no varchar(30), religion varchar(30), category varchar(30), income varchar(30),education varchar (30), occcupation varchar(60) ,pan varchar(30),aadhar varchar(60),seniorcitizen varchar(60),exisiting_account varchar(60));

select * from signuptwo;

create table signupthree(form_no varchar(30), account_Type varchar(30), card_number varchar(30), pin varchar(30),facility varchar (300) );
select * from signupthree;

create table login(form_no varchar(30), card_number varchar(30),pin varchar(30));
select * from login;
create table bank(pin varchar(30),date varchar(30), type varchar(30),amount varchar(30));
SELECT * from bank;

