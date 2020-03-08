---
layout: cosql
permalink: cosql
---

  <div class="navbar navbar-default navbar-fixed-top" id="topNavbar" role="navigation">
     <div class="container clearfix">
        <div class="leftNav">
           <div class="brandDiv">
              <a href="https://yale-lily.github.io/"><img src="/lily-logo.png" alt="test image" height="40"></a>
           </div>
        </div>
     </div>
  </div>
  <div class="cover" id="topCover">
     <div class="container">
        <div class="row">
           <div class="col-md-12">
              <h1 id="appTitle">
                 <img src="/images/yale_logo.png" alt="test image" height="60">
                 <img src="/images/salesforce_logo.png" alt="test image" height="65">
                 CoSQL
                 <b>1.0</b>
                 <img src="/images/cornell_logo.png" alt="test image" height="70">
                 <img src="/images/umichi_logo.png" alt="test image" height="70">
              </h1>
           </div>
           <h2 id="appSubtitle">A Conversational Text-to-SQL Challenge <br>Towards Cross-Domain Natural Language Interfaces to Databases</h2>
        </div>
     </div>
  </div>
  <div class="cover" id="contentCover">
     <div class="container">
        <div class="row">
           <div class="col-md-5">
              <div class="infoCard">
                 <div class="infoBody">
                    <div class="infoHeadline">
                       <h2>What is CoSQL?</h2>
                    </div>
                    <p align="left">
                    <div class="left"><b><i>CoSQL</i></b> is a corpus for building cross-domain <b>Co</b>nversational text-to-<b>SQL</b> systems. It is the dilaogue version of the <a href="https://yale-lily.github.io/spider"><b><i>Spider</i></b></a> and <a href="https://yale-lily.github.io/sparc"><b><i>SParC</i></b></a> tasks. CoSQL consists of 30k+ turns plus 10k+ annotated SQL queries, obtained from a <a href="https://en.wikipedia.org/wiki/Wizard_of_Oz_experiment">Wizard-of-Oz</a> collection of 3k dialogues querying 200 complex databases spanning 138 domains. Each dialogue simulates a real-world DB query scenario with a crowd worker as a user exploring the database and a SQL expert retrieving answers with SQL, clarifying ambiguous questions, or otherwise informing of unanswerable questions.
                    </div>
                    <a class="btn actionBtn" href="https://arxiv.org/abs/1909.05378">CoSQL Paper (EMNLP'19)</a>
                    <a class="btn actionBtn" href="https://medium.com/@tao.yu/spider-one-more-step-towards-natural-language-interfaces-to-databases-62298dc6df3c">CoSQL Post</a>
                    <hr><b>Related challenges</b>: single-turn <a href="https://yale-lily.github.io/spider"><b><i>Spider</i></b></a> and multi-turn <a href="https://yale-lily.github.io/sparc"><b><i>SParC</i></b></a> text-to-SQL tasks
                        <a class="btn actionBtn2" href="https://yale-lily.github.io/spider">Spider Chanllenge (EMNLP'18)</a>
                        <a class="btn actionBtn2" href="https://yale-lily.github.io/sparc">SParC Chanllenge (ACL'19)</a>
                    </p>
                    <div class="infoHeadline">
                       <h2>News</h2>
                    </div>
                    <p align="left">
                    <div class="left" style="background-color: #f5f5f5">
                       <ul>
                         <li><span class="label label-default" style="background-color: #286dc0"><i>01/16/2020</i></span>
                             Added some supplemental files to the CoSQL dataset (No change to the data content for each task).
                          </li>
                         <li><span class="label label-default" style="background-color: #286dc0"><i>10/30/2019</i></span>
                             CoSQL dataset is out, see you at <a href="https://www.emnlp-ijcnlp2019.org/">EMNLP 2019, Hong Kong</a>!
                          </li>
                       </ul>
                    </div>
                    </p>
                    <div class="infoHeadline">
                       <h2>Why CoSQL?</h2>
                    </div>
                    <p align="left">
                    <div class="left">
                       CoSQL introduces new challenges compared to existing task-oriented dialogue tasks:       
                       <ul>
                          <li>the dialogue states are grounded in domain-independent SQL program instead of domain-specific slot-value pairs.</li>
                          <li>because testing is done on unseen databases, success requires generalizing to new domains.</li>
                       </ul>
                    <hr>Compared to other semantic parsing/text-to-SQL tasks, CoSQL presents new challenges:
                       <ul>
                          <li>user questions are not necessarily answerable.</li>
                          <li>it involves system responses to clarify ambiguous questions, verify returned results, and notify users of unanswerable or unrelated questions.</li>
                          <li>each dialog is obtained via the Wizard-of-Oz setting between a crowd worker and a SQL expert.</li>
                       </ul>
                    <hr>CoSQL includes three tasks:
                      <ul>
                          <li><b>SQL-grounded dialogue state tracking</b> to map user utterances into SQL queries if possible given the interaction history</li>
                          <li><b>natural language response generation</b> based on an executed SQL and its results for user verification</li>
                          <li><b>user dialogue act prediction</b> to detect and resolve ambiguous and unanswerable questions</li>
                       </ul>
                    </div>
                    </p>
                    <div class="infoHeadline">
                       <h2>Getting Started</h2>
                    </div>
                    <p align="left">
                    <div class="left"> The data is split into training, development, and unreleased test sets. Download a copy of the dataset (distributed under the <a href="https://creativecommons.org/licenses/by-sa/4.0/legalcode">CC BY-SA 4.0</a> license):
                    </div>
                    </p>
                    <a class="btn actionBtn inverseBtn" href="https://drive.google.com/uc?export=download&id=14x6lsWqlu6gR-aYxa6cemslDN3qT3zxP" download>CoSQL Dataset</a>
                    Details of baseline models and evaluation script can be found on the following GitHub site:
                    <a class="btn actionBtn inverseBtn" href="https://github.com/taoyds/cosql" download>CoSQL GitHub Page</a>
                    <p align="left">
                    <div class="left">Once you have built a model that works to your expectations on the dev set,
                       you can submit it to get official scores on the dev and a hidden test set. To preserve the
                       integrity of test results, we do not release the test set to the public. Instead, we request
                       you to submit your model so that we can run it on the test set for you. Here's a tutorial walking you through official evaluation of your model:
                    </div>
                    </p>
                    <a class="btn actionBtn inverseBtn" href="https://worksheets.codalab.org/worksheets/0x308e69603f284587aab34b8c09aee4f1" download>Submission Tutorial</a>
                    <div class="infoHeadline">
                       <h2>Data Examples</h2>
                    </div>
                    <p align="left">
                    <div class="left"> Some examples look like the following:
                    </div>
                    </p>
                    <img src="/images/cosql_example.png" alt="test image">
                    <div class="infoHeadline">
                       <h2>Have Questions or Want to Contribute ?</h2>
                    </div>
                    <p align="left">
                    <div class="left">Ask us questions at our <a href="https://github.com/taoyds/sparc/issues">Github issues page</a> or contact <a href="https://taoyds.github.io/">Tao Yu</a>, <a href="https://ryanzhumich.github.io/">Rui Zhang</a>, or
                       <a href="http://victorialin.net/">Xi Victoria Lin</a>.
                    </div>
                    </p>
                    <p align="left">
                    <div class="left">We expect the dataset to evolve. We would greatly appreciate it if you could donate us your non-private databases or SQL queries for the project.
                    </div>
                    </p>
                    <div class="infoHeadline">
                       <h2>Acknowledgement</h2>
                    </div>
                    <p align="left">
                    <div class="left">We thank <a href="https://rajpurkar.github.io/">Pranav Rajpurkar</a> for giving us the permission to build this website based on <a href="https://rajpurkar.github.io/SQuAD-explorer/">SQuAD</a>.
                    </div>
                    </p>
                    <p align="left">
                    <div class="left">Part of our CoSQL team at <a href="https://yins.yale.edu/">YINS</a>:
                    </div>
                    </p>
                    <img src="/images/sparc_lily.jpeg" alt="test image">
                 </div>
              </div>
           </div>
           <div class="col-md-7">
              <div class="infoCard">
                 <div class="infoBody">
                    <div class="infoHeadline">
                       <h2>Leaderboard - SQL-grounded Dialogue State Tracking</h2>
                    </div>
                    <p align="left">
                    <div class="left">In CoSQL, user dialogue states are grounded in SQL queries. Dialogue state tracking (DST) in this case is to predict the correct SQL query for each user utterance with <code>INFORM_SQL</code> label given the interaction context and the DB schema. Comparing to other context-dependent text-to-SQL tasks such as <a href="https://yale-lily.github.io/sparc"><i>SParC</i></a>, the DST task in CoSQL also includes the ambiguous questions if the user affirms the system clarification of them. In this case, the system clarification is also given as part of the interaction context to predict the SQL query corresponding to the question. As in <a href="https://yale-lily.github.io/spider"><i>Spider</i></a> and <a href="https://yale-lily.github.io/sparc"><i>SParC</i></a> tasks, we report results of Exact Set Match without Values here.
                    </div>
                    </p>
                    <table class="table performanceTable">
                        <tr>
                           <th>Rank</th>
                           <th>Model</th>
                           <th>Question Match</th>
                           <th>Interaction Match</th>
                        </tr>
                        <tr>
                           <td>
                              <p>1</p>
                              <span class="date label label-default">Aug 30, 2019</span>
                           </td>
                           <td style="word-break:break-word;">
                              EditSQL
                              <p class="institution">Yale University & Salesforce Research</p>
                              <a class="link" href="https://arxiv.org/abs/1909.00786">(Zhang et al. EMNLP '19)</a>
                              <a class="link" href="https://github.com/ryanzhumich/editsql">code</a>
                           </td>
                           <td><b>40.8</b></td>
                           <td><b>13.7</b></td>
                        </tr>
                        <tr>
                           <td>
                              <p>2</p>
                              <span class="date label label-default">Aug 30, 2019</span>
                           </td>
                           <td style="word-break:break-word;">
                              CD-Seq2Seq
                              <p class="institution">Yale University & Salesforce Research</p>
                              <a class="link" href="https://arxiv.org/abs/1909.05378">(Yu et al. EMNLP '19)</a>
                              <a class="link" href="https://github.com/ryanzhumich/editsql">code</a>
                           </td>
                           <td>13.9</td>
                           <td>2.6</td>
                        </tr>
                        <tr>
                           <td>
                              <p>3</p>
                              <span class="date label label-default">Aug 30, 2019</span>
                           </td>
                           <td style="word-break:break-word;">
                              SyntaxSQL-con
                              <p class="institution">Yale University</p>
                              <a class="link" href="https://arxiv.org/abs/1810.05237">(Yu et al. EMNLP '18)</a>
                              <a class="link" href="https://github.com/taoyds/syntaxSQL">code</a>
                           </td>
                           <td>14.1</td>
                           <td>2.2</td>
                        </tr>
                    </table>
                 </div>
              </div>
              <div class="infoCard">
                 <div class="infoBody">
                    <div class="infoHeadline">
                       <h2>Leaderboard - Response Generation from SQL and Query Results</h2>
                    </div>
                    <p align="left">
                    <div class="left"> This task requires generating a natural language description of the SQL query and the result for each system response labeled as <code>INFORM_SQL</code>. It considers a SQL query, the execution result, and the DB schema. Preserving logical consistency (Logic Correctness Rate (LCR)) between SQL and NL response is crucial in this task, in addition to naturalness and syntactical correctness.
                    </div>
                    </p>
                    <table class="table performanceTable">
                    <tr>
                       <th>Rank</th>
                       <th>Model</th>
                       <th>BLEU</th>
                       <th>Grammar</th>
                       <th>LCR (%)</th>
                    </tr>
                    <tr>
                       <td>
                          <p>1</p>
                          <span class="date label label-default">Aug 30, 2019</span>
                       </td>
                       <td style="word-break:break-word;">
                          Template baseline
                       </td>
                       <td>9.3</td>
                       <td>4.0</td>
                       <td>41.0</td>
                    </tr>
                    <tr>
                       <td>
                          <p>2</p>
                          <span class="date label label-default">Aug 30, 2019</span>
                       </td>
                       <td style="word-break:break-word;">
                          Pointer-generator baseline
                       </td>
                       <td>15.1</td>
                       <td>3.6</td>
                       <td>35.0</td>
                    </tr>
                    <tr>
                       <td>
                          <p>3</p>
                          <span class="date label label-default">Aug 30, 2019</span>
                       </td>
                       <td style="word-break:break-word;">
                          Seq2Seq baseline
                       </td>
                       <td>14.1</td>
                       <td>3.5</td>
                       <td>27.0</td>
                    </tr>
                    </table>
                 </div>
              </div>
              <div class="infoCard">
                 <div class="infoBody">
                    <div class="infoHeadline">
                       <h2>Leaderboard - User Dialogue Act Prediction</h2>
                    </div>
                    <p align="left">
                    <div class="left"> For a real-world DB querying dialogue system, it has to decide if the user question can be mapped to a SQL query or if special actions are needed. We define a series of dialogue acts for the DB user and the SQL expert (refer to the paper for more details). For example, if the user question can be answered by a SQL query, the dialogue act of the question is <code>INFORM_SQL</code>.
                    </div>
                    </p>
                    <table class="table performanceTable">
                    <tr>
                       <th>Rank</th>
                       <th>Model</th>
                       <th>Accuracy</th>
                    </tr>
                    <tr>
                       <td>
                          <p>1</p>
                          <span class="date label label-default">Dec 20, 2019</span>
                       </td>
                       <td style="word-break:break-word;">
                          UTran-SQL
                       </td>
                       <td><b>87.2</b></td>
                    </tr>
                    <tr>
                       <td>
                          <p>2</p>
                          <span class="date label label-default">Aug 30, 2019</span>
                       </td>
                       <td style="word-break:break-word;">
                          TBCNN-pair baseline
                       </td>
                       <td>83.9</td>
                    </tr>
                    <tr>
                       <td>
                          <p>3</p>
                          <span class="date label label-default">Aug 30, 2019</span>
                       </td>
                       <td style="word-break:break-word;">
                          Majority baseline
                       </td>
                       <td>62.8</td>
                    </tr>
                    </table>
                 </div>
              </div>
           </div>
        </div>
     </div>
  </div>