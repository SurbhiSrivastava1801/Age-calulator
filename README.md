<html>

<head>
    <style type="text/css">
        body {
            background-color: lightsalmon;
        }
    </style>
    
</head>


</html>
<html>

<head>
    <script>
        function ageCalculator() {
            var userinput = document.getElementById("DOB").value;
            var dob = new Date(userinput);
            if (userinput == null || userinput == '') {
                document.getElementById("message").innerHTML = "**Choose a date please!";
                return false;
            } else {

                var dobYear = dob.getYear();
                var dobMonth = dob.getMonth();
                var dobDate = dob.getDate();


                var now = new Date();

                var currentYear = now.getYear();
                var currentMonth = now.getMonth();
                var currentDate = now.getDate();


                var age = {};
                var ageString = "";


                yearAge = currentYear - dobYear;


                if (currentMonth >= dobMonth)

                    var monthAge = currentMonth - dobMonth;
                else {
                    yearAge--;
                    var monthAge = 12 + currentMonth - dobMonth;
                }


                if (currentDate >= dobDate)

                    var dateAge = currentDate - dobDate;
                else {
                    monthAge--;
                    var dateAge = 31 + currentDate - dobDate;

                    if (monthAge < 0) {
                        monthAge = 11;
                        yearAge--;
                    }
                }

                age = {
                    years: yearAge,
                    months: monthAge,
                    days: dateAge
                };


                if ((age.years > 0) && (age.months > 0) && (age.days > 0))
                    ageString = age.years + " years, " + age.months + " months, and " + age.days + " days old.";
                else if ((age.years == 0) && (age.months == 0) && (age.days > 0))
                    ageString = "Only " + age.days + " days old!";

                else if ((age.years > 0) && (age.months == 0) && (age.days == 0))
                    ageString = age.years + " years old. Happy Birthday!!";
                else if ((age.years > 0) && (age.months > 0) && (age.days == 0))
                    ageString = age.years + " years and " + age.months + " months old.";
                else if ((age.years == 0) && (age.months > 0) && (age.days > 0))
                    ageString = age.months + " months and " + age.days + " days old.";
                else if ((age.years > 0) && (age.months == 0) && (age.days > 0))
                    ageString = age.years + " years, and" + age.days + " days old.";
                else if ((age.years == 0) && (age.months > 0) && (age.days == 0))
                    ageString = age.months + " months old.";

                else ageString = "Welcome to Earth! <br> It's first day on Earth!";


                return document.getElementById("result").innerHTML = ageString;

            }
        }
    </script>
</head>

<body>
    <center>
        <h2 style="color: 32a80f" align="center"> Calculate Age from Date of Birth <br> <br> </h2>

        <b> Enter Date of Birth: <input type=date id=DOB>  </b>
        <span id="message" style="color:red"> </span> <br><br>
        <button type="submit" onclick="ageCalculator()"> Calculate age </button> <br><br>
        <h3 style="color:32a80f" id="result" align="center"></h3>
    </center>
</body>

</html>
<br>
<html>

<head>
    <style type="text/css">
        h4 {
            font-size: x-large;
            font-family: Georgia, 'Times New Roman', Times, serif;
        }
    </style>
    <style type="text/css">
        h3 {
            font-family: 'Times New Roman', Times, serif;
            font-weight: lighter;
            font-family: Georgia, 'Times New Roman', Times, serif;
        }
    </style>
    <style type="text/css">
        h5 {
            font-size: x-large;
            font-family: Georgia, 'Times New Roman', Times, serif;
        }
    </style>
    <style type="text/css">
        h6 {
            font-size: x-large;
            font-family: Georgia, 'Times New Roman', Times, serif;
        }
    </style>
    <style type="text/css">
        h7 {
            font-size: x-large;
            font-family: Georgia, 'Times New Roman', Times, serif;
        }
    </style>
    <style type="text/css">
        h8 {
            font-size: x-large;
            font-family: Georgia, 'Times New Roman', Times, serif;
        }
    </style>
    <style type="text/css">
        a:link {
            color: royalblue;
        }
        
        a:hover {
            color: seagreen;
        }
        
        a:active {
            color: red;
        }
    </style>
    <style type="text/css">
        #para1 {
            font-size: x-large;
            text-align: center;
        }
    </style>
</head>

<body>
    <ul>
        <li> <a href="#About me"> About me</a> </li>
        <li> <a href="#reason for this homepage"> motivation for making homepage </a> </li>


    </ul>
    <h8>
        <u>ABOUT AGE CALCULATOR</u>
    </h8>
    <P>
        The age of a person can be counted differently in different cultures. This calculator is based on the most common age system. In this system, age grows at the birthday. For example, the age of a person that has lived for 3 years and 11 months is 3 and
        the age will turn to 4 at his/her next birthday one month later. Most western countries use this age system.
    </P>
    <p>
        In some cultures, age is expressed by counting years with or without including the current year. For example, one person is twenty years old is the same as one person is in the twenty-first year of his/her life. In one of the traditional Chinese age systems,
        people are born at age 1 and the age grows up at the Traditional Chinese New Year instead of birthday. For example, if one baby was born just one day before the Traditional Chinese New Year, 2 days later the baby will be at age 2 even though he/she
        is only 2 days old. In some situations, the months and days result of this age calculator may be confusing, especially when the starting date is the end of a month. For example, we all count Feb. 20 to March 20 to be one month.
    </p>
    <p>
        However, there are two ways to calculate the age from Feb. 28, 2015 to Mar. 31, 2015. If thinking Feb. 28 to Mar. 28 as one month, then the result is one month and 3 days. If thinking both Feb. 28 and Mar. 31 as the end of the month, then the result is
        one month. Both calculation results are reasonable. Similar situations exist for dates like Apr. 30 to May 31, May 30 to June 30, etc. The confusion comes from the uneven number of days in different months. In our calculation, we used the former
        method.

    </P>
    <h5>
        what is Age calcuator..?
    </h5>

    <p>
        The Age Calculator can determine the age or interval between two dates.<br> The calculated age will be displayed in years, months, weeks, days, hours, minutes, and seconds.<br> The age of a person can be counted differently in different cultures.<br>        This calculator is based on the most common age system.
    </p>
    <h6>
        <u>Uses of AGE CALCULATOR</u>
    </h6>
    <p>
        The main reason of using the online age calculator is because it is taking less time <br> and also gives correct result. So this Age calculator online is tool which calculates date <br> of birth to current date online and also age calculated from
        date of birth <br> it can calculate.
    </p>
    <h7>
        how I made this ONline AGE Calculator...!
    </h7>
    <p>
        I made this AGE CALCULATOR as my SOC(season of Code) project with the help pf coding.<br> in this coding i used following programming languages.<br>
        <ul>
            <li>HTML</li>
            <li>CSS</li>
            <li>JAVASCRIPT</li>
        </ul>
        for which i first made an GITHUB ACCOUNT <a href="https://github.com/SurbhiSrivastava1801">link</a><br> then i have downloaded Visual Studio code.<br> then i made a repositery in github and clone it to vs code.
    </p>
    <h4> <u>ABOUT ME </u></h4>
    <style type="text/css">
        p {
            font-size: inherit;
            text-align: left;
            letter-spacing: 1.5px;
            line-height: 20px;
        }
    </style>
    <p>
        <a name="About me">
            Hey evryone,
            I am Surbhi Srivastava a 1st year undergraduate at IIT BOMBAY. <br>
            Mechanical engineering department dual degree program basically interested in learning programing languages. <br>
            my hobbies are eating ,sleeping, and <br>
            watching movies (although i don't get time for it now :( ).
            <br>
        </a>
    </p>
    <p>
        contact me at
        <ul>
            <li> <a href="https://www.facebook.com/surbhi.srivastava.10888/"> Facebook id </a> </li>
            <li> <a href="srivastava1801@gmail.com"> srivastava1801@gmail.com </a> </li>
        </ul>
    </p>
    <h3> This is me </h3>
    <p id="para1"> <img src="me.jpeg" width="400" height="400"> </p>

    <h4><u> MOTIVATION FOR MAKING HOMEPAGE</u> </h4>
    <p> <a name="reason for this homepage"> I have participated in SOC and as a part of this project <br> i am doing this to learn my weak was to rush with two upcoming quizzes its mid night saturdayy and i have to submit my assignment before 12 noon and i am loving it :) </a>        </p>
</body>

</html>
