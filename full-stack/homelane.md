The Ultimate FIFA Dream Team Selection Challenge

[Problem Statement]

For the new season of English Premier League, the football club owners are re-strategizing their teams to ensure that they win this season. They need crunch data to build their dream team and guarantee a win. You are required to help the coaches who are not very tech savvy make a quick and effective decision by retrieving the data that they require.

In order to help them, you are required to implement a backend system for FIFA. This system must implement the following:

    Microservices architecture that extracts the provided data  

    Microservices APIs for the quick retrieval of the data

The dataset that is provided is an extensive dataset of the football players with the following details:

    Personal details (e.g. Name, Age, Photo,  Value, Wage)

    Affiliations (e.g. Nationality, Flag, Club, Club Logo)

    Stats (e.g. Shot power, Sliding tackle, Sprint speed, Stamina, Standing tackle, Strength, Vision, Heading accuracy, Interceptions, Jumping, Long passing, Long shots, Marking, Penalties,  Free kick accuracy)

    Traits (e.g. Preferred Positioning, Aggression, Agility, Balance, Ball control, Composure)

    Overall Potential

There are four tables which you must add to your database.

 

[Tasks]

    Dump the FIFA data set that is provided into your MySQL database and create the required schema.

    Implement at least two microservices for the following:

        Authentication of the incoming request. Implement API key authentication to validate users.

        Querying the database. You have to create SQL queries from JSON input.

    Query Service: This should be the only user-facing service that can be called using an API endpoint. Implement the API key authentication for this service. This service should do the following:

        Take input and provide output in the JSON format. You are expected to create your own JSON Schema for input and output.

        Validate the API key and JSON schema

        Post validation, this should internally call the data-retrieval service

    Data Service: This service is not user-facing and should restrict access to certain predefined IP addresses. This Service can only be invoked from internal machines of the private network and not from the public web. The primary task of this API is to query the database. It should do the following:

        Takes complex JSON (nested JSON) as input and creates a complex SQL to query data from many tables.

        Feed the resultset to the first service

[Required APIs]

Implement at least three APIs for the Query Service:

    get_player_info(player_name)

        This API should take player_name as the input and retrieve extensive data about that player from the database.

        The data should contain the player’s personal details , stats, affiliations, traits  and overall potential.
         

    get_club_player_list(club_name)

        This API retrieves the names of all the players who play for a specific club.

        It should take club_name as the input and retrieve extensive data about all the players who play for that club.  

        The data should contain all the player’s personal details, stats, affiliations, traits and overall potential.

     

 

[Brownie points]

    For get_player_info (player_name) API

        If more than one players match the player_name, sort the retrieved entries in the order of (1) Years of experience, and further sorted by (2) Number of matches played and (3) Overall potential.

    Implement the following API

strengthen_team(club_name): This is an analysis API which retrieves all the players for different positions who need improvement.

        Assume that the base rating for every position in the team should be 80 or more. For every position in the team whose base rating is <80, recommend players from other teams/clubs along with their wage and value. E.g positions: ST: Strikes, CF: Center Forward, CAM: Center Attacking midfielder. All of these are provided in the database.

    Implement an API that takes custom input like querying more than one player in JSON (get_player_info(player_name1, player_name2, ...)

    Test code for automated testing of the two services

 

[Guide]

    Fifa Data-dump: http://hck.re/ml8ZJ6

    TechStack

        Java/Kotlin

        RxJava

        NodeJS

        PHP

        MySQL

 

[Submission Instructions]

    Zip your source code, deployment instructions, and upload the zipped file.

Note: The code must build and run without any intervention from the evaluators.

    Comment your code well for ease of assessment.

    Explain the logic behind your choices in an accompanying document.
