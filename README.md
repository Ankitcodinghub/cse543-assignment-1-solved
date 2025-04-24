# cse543-assignment-1-solved



**<span style='color:red'>TO GET THIS SOLUTION VISIT:</span>** https://www.ankitcodinghub.com/product/cse543-information-assurance-and-security-udp-spoofing-assignment-solved/

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;126197&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSE543 Assignment 1 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">
            
<div class="kksr-stars">
    
<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
    
<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>
                

<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
<h1>Purpose</h1>
The purpose of this assignment is to make you feel comfortable with using a VPN connection and working directly with raw sockets. You will learn how to create and use raw sockets, send raw IP packets with forged source IPs, and manually create UDP packets.

<h1>Objectives</h1>
Learners will be able to:

<ul>
<li>Program with raw sockets.</li>
<li>Create UDP packets manually and programmatically.</li>
<li>Send UDP packets with spoofed source IP addresses.</li>
</ul>
<h1>Technology Requirements</h1>
While learners can use any programming language, Python is strongly recommended.

<strong>Note</strong>: The course team will not be able to help you if you choose any language that is not Python, Java, or C#; therefore, to create the best learning experience, Python is strongly recommended.

<h1>Assignment Description and Directions</h1>
<h2>Technology Setup Reminder</h2>
If you have not already joined the course’s pwn.college, please review the setup directions in <em>Module 0: Welcome and Start Here </em>of your course to properly gain access and start your work.

<h2>Accessing the Environment</h2>
<ol>
<li>Navigate to <a href="https://pwn.college/">https://pwn.college</a>.</li>
<li>Click “<strong>Login</strong>” in the upper right corner of the screen and enter your account credentials.
<ol>
<li>Click “Forgot your password?” if you have trouble logging in.</li>
</ol>
</li>
<li>Navigate to “<strong>Dojos</strong>”, second option from the left at the top of the screen.</li>
<li>Under “<strong>Courses</strong>”, select “<strong>CSE 543 – Session X Year</strong>”.</li>
<li>Under “<strong>Dojo Modules</strong>” and select “<strong>IA in Information Systems</strong>”.</li>
<li>Under “<strong>Challenges</strong>”, click on “<strong>UDPSpoof</strong>”, read the details, and then click “<strong>Start</strong>” when you are ready to work.
<ol>
<li>Optional: use “<strong>Practice</strong>” to help you work through the level with assistance.</li>
</ol>
</li>
</ol>
<h2>Assignment Directions</h2>
A UDP service FlagServ is running at 10.0.0.3:13337. This UDP service receives a target IP address from the user, and if the user is authenticated, it will happily send a flag (a special string) via UDP to port 13337 of the target IP. Your job is to write a program that retrieves the flag.

FlagServ employs THE BEST AUTHENTICATION METHOD IN THE WORLD: Source-IP-based

authentication, which means it authenticates all users based on their source IP addresses. If a user’s source IP address is trusted, FlagServ will send out the flag to the specified destination (repeat: via UDP). Otherwise, it will send an error message back to the untrusted user (via UDP, too).

The only trusted IP is 10.2.4.10. Your task is to break or bypass this source-IP-based authentication scheme and steal the flag.

To keep the internet a secure place, 10.0.0.3 points to a private IP that is only accessible in the pwn.college challenge environment.

<h1>Submission Directions for Assignment Deliverables</h1>
You are given an unlimited number of attempts to submit your best work. The number of attempts is given to anticipate any submission errors you may have in regards to properly submitting your best work within the deadline (e.g., accidentally submitting the wrong paper). It is not meant for you to receive multiple rounds of feedback and then one (1) final submission. Only your most recent submission will be assessed.

You must complete your UDP Spoofing Assignment deliverables in <strong>pwn.college </strong>and then <strong>submit the deliverables in its submission space in the course</strong>. Carefully review submission directions outlined in the overview document in order to correctly earn credit for your work. Learners may not email or use other means to submit any assignment or project for review, including feedback, and grading.

2

The UDP Spoofing Assignment includes two (2) deliverables<strong>:</strong>

<ul>
<li><strong>Readme</strong>: Include a <strong>txt file `readme.txt` </strong>describing your thought process or your solution to this problem.</li>
<li><strong>Program/Code</strong>: In a ZIP file, provide your code (a Python script or source code in any programming languages) that attacks the service and obtains the flag.</li>
</ul>
<h2>Making File Submissions in Canvas</h2>
Before submitting, confirm that your deliverables follow the requirements for the project, and then submit your work in the designated submission space in the course. Your submission will be reviewed by the course team and then, after the due date has passed, your score will be populated into your grade.

<ol>
<li>In your course, go to <strong>Submission: UDP Spoofing Assignment</strong>.</li>
<li>Click <strong>Start Assignment</strong>.</li>
<li>Click <strong>Choose File</strong>.</li>
<li>Locate and select <strong>one (1) </strong>deliverable file from your device.</li>
<li>If needed, click <strong>+Add Another File </strong>and repeat Steps 3 and 4 until all deliverables are added.</li>
<li>Select the <strong>agreement </strong>and then click <strong>Submit Assignment</strong>.</li>
<li>(If needed and allowed) To resubmit files:</li>
<li>Return to the Canvas submission space, click <strong>New Attempt</strong>, and repeat the process from Step 3.</li>
</ol>
<h1>Evaluation</h1>
Your submission will be automatically graded in the challenge environment. When you complete the assignment’s challenge, you will receive a score in pwn.college. After the due date passes, the score will be reviewed by the course team, aligned with the course grade breakdown, and then populated in your course grade in Canvas. For example, if you earn 100% on the challenge in pwn.college, you will earn the maximum number of points for the corresponding assignment in Canvas. Please refer to the syllabus PDF and the assignment submission space in Canvas so you know how many points each assignment is worth.

<ul>
<li>You will earn full credit if you steal and submit the correct flag.</li>
<li>If you do not steal and submit the correct flag, you will not earn credit.</li>
<li>Partial credit will not be granted for this assignment.</li>
</ul>
3
