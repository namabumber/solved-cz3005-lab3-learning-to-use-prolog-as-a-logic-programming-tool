Download Link: https://assignmentchef.com/product/solved-cz3005-lab3-learning-to-use-prolog-as-a-logic-programming-tool
<br>
<strong>Learning to Use Prolog as a Logic Programming Tool </strong>

<table width="601">

 <tbody>

  <tr>

   <td width="160"><strong>Learning Objective: </strong></td>

   <td width="441">To reinforce the understanding on the use of Prolog as a tool of logic programming and the specification of declarative knowledge – semantic information.<strong> </strong></td>

  </tr>

  <tr>

   <td width="160"><strong>Learning Outcome: </strong></td>

   <td width="441">a)     Understand the separation of Knowledge from the inference mechanism in Knowledge-Based System (KBS).b)    Understand that the proof procedure is based on the refutational proof using resolution on Horn Clauses.c)     Appreciate the ordering of the clauses of the same class affects the proof sequence. </td>

  </tr>

  <tr>

   <td width="160"><strong>Tools: </strong></td>

   <td width="441">SWI-Prolog – <a href="http://www.swi-prolog.org/">http://www.swi</a><a href="http://www.swi-prolog.org/">–</a><a href="http://www.swi-prolog.org/">prolog.org/</a></td>

  </tr>

  <tr>

   <td width="160"><strong>Learning Activities: </strong></td>

   <td width="441">1.     Download and install SWI-Prolog.2.     Watch the two briefing videos on NTULearn:a.    “<strong>Prolog (1.Introduction).mp4</strong>”b.    “<strong>Prolog (2.Building a KB).mp4</strong>“.These two videos explain the details in the guide on “<strong>How to Program in Prolog.pdf</strong>“. </td>

  </tr>

  <tr>

   <td width="160"><strong>Deliverables: </strong></td>

   <td width="441">This assignment consists of two problems. You are to specify each of them as a declarative knowledge base in Prolog. </td>

  </tr>

  <tr>

   <td width="160"><strong>Submission Instruction: </strong></td>

   <td width="441">Complete both Exercise 1 and Exercise 2. Your submission should contain:1)      The Prolog knowledge bases (A“&lt;your_name&gt;_qn_1_2.pl” file for Exercise 1.2, a“&lt;your_name&gt;_qn_2_1.pl” file for Exercise 2.1 and a“&lt;your_name&gt;_qn_2_2.pl” file for Exercise 2.2), and2)      A brief report in PDF format“&lt;your_name&gt;_Assignment3.pdf” showing the:a.    FOL statements (where required by the question),b.    Traces of the queries for the two questions. You should include your name, tutorial group number (e.g., TSR1) and matriculation card number in the cover page of your report. The submission is through NTULearn. The deadline for submission is by Week 12 (<strong>Thursday, 11:59pm, 05 November 2020</strong>). </td>

  </tr>

 </tbody>

</table>

<strong>         </strong>

<strong>[Quick References] </strong>Key syntax of Prolog:

<ol>

 <li>Defining a fact: <strong>P(X). </strong></li>

</ol>

For example: male(peter). “Peter is a male”.

<ol start="2">

 <li>Defining a relationship: <strong>R(X,Y).</strong></li>

</ol>

For example, sister(anne, mary). “Anne is a sister of Mary”.

<ol start="3">

 <li>Defining a conjunctive (AND) sentence: <strong>Goal :- Premise 1, Premise 2, …, Premise N.</strong> For example, mother_of(X,Y) :- child_of(Y,X), female(X), X = Y. “X is the mother of</li>

</ol>

Y if Y is the child of X and X is female and X is not Y”.

<ol start="4">

 <li>Defining a disjunctive (OR) sentence: <strong>Goal :- Premise 1; Premise 2; …; Premise N.</strong> For example, lose_weight(X) :- eat_less(X); exercise_more(X). “X loses weight if X eats less or X exercises more”.</li>

 <li>How to produce a <strong>trace</strong>:</li>

</ol>

In the Prolog command line interface, type <strong>trace,</strong> before entering your query. Then, press <strong>&lt;enter&gt;</strong> to trace step-by-step. For example:<strong>          </strong>

<strong>Exercise 1: The Smart Phone Rivalry</strong>sumsum, a competitor of appy, developed some nice smart phone technology called galacticas3, all of which was stolen by stevey, who is a boss. It is unethical for a boss to steal business from rival companies. A competitor of appy is a rival. Smart phone technology is business.

<ol>

 <li>Translate the natural language statements above describing the dealing within the Smart Phone industry in to First Order Logic (FOL).</li>

</ol>

(5 marks) 2. Write these FOL statements as Prolog clauses.

(5 marks) 3. Using Prolog, prove that Stevey is unethical. Show a trace of your proof.

<h1>Exercise 2: The Royal Family</h1>

The old Royal succession rule states that the throne is passed down along the male line according to the order of birth before the consideration along the female line – similarly according to the order of birth. queen elizabeth, the monarch of United Kingdom, has four offsprings; namely:- prince charles, princess ann, prince andrew and prince edward – listed in the order of birth.

<ol>

 <li>Define their relations and rules in a Prolog rule base. Hence, define the old Royal succession rule. Using this old succession rule determine the line of succession based on the information given. Do a trace to show your results.</li>

 <li>Recently, the Royal succession rule has been modified. The throne is now passed down according to the order of birth irrespective of gender. Modify your rules and Prolog knowledge base to handle the new succession rule. Explain the necessary changes to the knowledge needed to represent the new information. Use this new succession rule to determine the new line of succession based on the same knowledge given. Show your results using a trace.</li>

</ol>

<strong>[</strong><strong><u>Important</u>]</strong> <em>Prolog interprets capital lettered words as variables. Thus, in your Prolog code, please write the above terms in </em><em>blue using all lower-case letters. </em>