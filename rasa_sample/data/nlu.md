## intent:greet
- hey
- hello
- hi
- good morning
- good evening
- hey there

## intent:goodbye
- bye
- goodbye
- see you around
- see you later

## intent:affirm
- yes
- indeed
- of course
- that sounds good
- correct

## intent:deny
- no
- never
- I don't think so
- don't like that
- no way
- not really

## intent:mood_great
- perfect
- good
- very good
- great
- amazing
- wonderful
- I am feeling very good
- I am great
- I'm good

## intent:mood_unhappy
- sad
- very sad
- unhappy
- bad
- very bad
- awful
- terrible
- not very good
- extremely sad
- so sad

## intent:bot_challenge
- are you a bot?
- are you a human?
- am I talking to a bot?
- am I talking to a human?

## intent:affirm
- y
- Y
- ya
- yes
- yes sure
- absolutely
- for sure
- yes yes yes
- definitely
- yes, it did.
- yes
- yeah

## intent:deny
- no
- never
- nope
- I don't think so
- don't like that
- no way
- not really
- n
- N

## intent:thanks
- Thanks
- Thank you
- Thank you so much
- Thanks bot
- Thanks for that
- cheers
- cheers bro
- ok thanks!
- perfect thank you
- thanks a bunch for everything
- thanks for the help
- thanks a lot
- amazing, thanks
- cool, thanks
- cool thank you
- thanks

## intent:goodbye
- Bye
- Goodbye
- See you later
- Bye bot
- Goodbye friend
- bye
- bye for now
- catch you later
- gotta go
- See you
- goodnight
- have a nice day
- i'm off
- see you later alligator
- we'll speak soon
- end
- finish

## intent:greet
- Hi
- Hey
- Hi bot
- Hey bot
- Hello
- Good morning
- hi again
- hi folks
- hi Mister
- hi pal!
- hi there
- greetings
- hello everybody
- hello is anybody there
- hello robot
- who are you?
- what are you?
- what's up
- how do you do?
- hi, this is [jill](PERSON)
- hello, this is [steven](PERSON)
- hey, my name is [steven](PERSON)
- hola, this is [john](PERSON)
- hey, my name is [steven](PERSON)
- hey, I am [Jack](PERSON)
- hey, my name is [steven](PERSON)
- hello, [steven](PERSON) is my name
- hi

## intent:position
- I’d like to know which positions are open right now
- Can I know about open positions?
- Do you have [any](roletype) openings?
- Do you have [any](roletype) opportunities available?
- I would like to get a job with you
- do you have jobs
- I want to join your company
- A [technical](role_type) one
- A [business](role_type) one
- A [tech](role_type:technical) one
- A [management](role_type:business) one
- [technology](role_type:technical)
- [tech](role_type:technical)
- [management](role_type:business)
- [business](role_type)
- Can I see some of the [business](role_type) roles?
- Can I see some of the [technical](role_type) roles?
- Can I see some of the [tech](role_type:technical) roles?
- Can I seeking [tech](role_type:technical) roles?
- Do you have opening in [tech](role_type:technical)?
- how about [tech](role_type:technical)?
- show me [tech](role_type:technical) roles
- can i know about open positions?
- [technical](role_type)
- tell me about open positions
- do you have any vacancies
- [anything](role_type:any)
- [anything](role_type:any) is fine
- I am open to [anything](role_type:any)
- position
- [any](roletype) role
- [any](roletype)

## intent:greet+position
- Hi,Can I know about open positions?
- Hey, Do you have any openings?
- Hi bot, do you have any vacancies
- Hey bot, I’d like to know which positions are open right now
- Hello, Can I know about open positions?
- hi again, I would like to get a job with you
- hi folks, Can I know about open positions?
- hi Mister,Do you have any openings?
- hi pal! tell me about open positions
- hi there,Can I know about open positions?
- greetings, do you have jobs
- hello everybody,I would like to get a job with you
- hello is anybody there, Can I know about open positions?


## intent:name
- My name is [sam](PERSON)
- My name is [sam paul](PERSON)
- I am [Paul](PERSON)
- I am [paul thomas](PERSON)
- My name is [George](PERSON)
- My name is [george xavier](PERSON)
- This is [Mary](PERSON)
- my name is [Niranjan](PERSON)
- i am [Sanjeeb](PERSON)
- myself [niranjan](PERSON)
- my name is [naresh](PERSON)
- [George](PERSON)
- [george](PERSON)
- [Mary john](PERSON)
- [mary](PERSON)
- [jibin mathew](PERSON)


## intent:give_email
- my email is [joe@aol.com](email)
- [123@123.co.uk](email)
- Email: [asdasd@asdasd.info](email)
- this is my email - [asd123@asd1.co.uk](email)
- here it is [123@123.co.uk](email)

## intent:give_tel
- my number is [9182736455](tel)
- contact me at [9338225664](tel)
- call me at [+853 9876 2345](tel)
- contact is [+44 7893096125](tel)
- tel number: [+33 9876 1234 083](tel)
- my contact is [+44 7893096125](tel)
- sure, my number is [+853 98762345](tel)
- [9861554423](tel)
- my no is [9334556734](tel)

## regex:email
- [\w-]+@([\w-]+\.)+[\w-]+

## regex:tel
- (0)([0-9][\s]*){10}

##intent:task
- how can you help me
- what can you do for me
- what do you do
- can you help
- what tasks you do
- how can you assist me
- how you can help me
- can you help me



