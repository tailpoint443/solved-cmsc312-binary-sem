Download Link: https://assignmentchef.com/product/solved-cmsc312-binary-sem
<br>
<ol>

 <li><strong>Prove/disprove that SJF is optimal in terms of average turnaround times of the processes. (2 points) </strong></li>

</ol>

SJF is an optimal algorithm because the wait time for short processes much more than it increases the wait time for long process.







<ol start="2">

 <li><strong>For what types of workloads does SJF deliver the same turnaround times as FIFO? (2 points) </strong></li>

</ol>

SJF has the best turnaround time in the most cases compared to FIFO and RR. The only time SJF has the same turnaround time as FIFO is when all the job has the same number of burst times. Also, when process P1 come in at 1 with 1 burst time, P2 comes in at 2 with 2 Burt time then the average turnaround time for FIFO and SJF will be the same.




<ol start="3">

 <li><strong>For what types of workloads and quantum lengths does SJF deliver the same response times as RR? (2 points) </strong></li>

</ol>

SJF will have same response times as RR when the quantum length of RR is larger than the largest burst time to be serviced and when the process arrives in order of increasing size.




<ol start="4">

 <li><strong>What happens to response time with SJF as job lengths increase? (2 points) </strong></li>

</ol>

In SJF if the job length increases, then the response time with SJF will increase too. The larger the increase, the greater the average response time will be for SJF.




<ol start="5">

 <li><strong>What happens to response time with RR as quantum lengths increase? Explain in words and write an equation that gives the worst-case response time, given N jobs. (2 points) </strong></li>

</ol>

When quantum lengths increase in RR, then response time increases because each process gets a small unit of CPU time and will be taken out of CPU then added to the end of the ready queue once the time has elapsed. Increasing the quantum length will just increase the waiting time for each process to be preempted and added. If there are n processes in the ready queue and the quantum length is q, then each process gets 1/n of the CPU time. A process has to wait at worst q(n-1) meaning the longer the quantum length, the longer the process waits.

<ol start="6">

 <li><strong>“Preemptive schedulers are always less efficient than non-preemptive schedulers.” Explain how this statement can be true if you define efficiency one way and how it is false if you define efficiency another way. (2 points) </strong></li>

</ol>

Preemptive schedulers are usually more efficient than non-preemptive schedulers because in non-preemptive scheduling, once the CPU cycle is allocated to process, the process holds it till it reaches a waiting state or terminated. In Preemptive SJF Scheduling, jobs are put into the ready queue as they come. In terms of efficiency, a preemptive scheduler would be considered less efficient than a non-preemptive scheduler because it has a higher overhead. It must switch out processes and change their states much more often. In the other hand, a preemptive scheduler will always have a faster response time compared to a non-preemptive scheduler that has to wait till one process completes before starting another while a preemptive scheduler can just switch to the processes necessary.




<ol start="7">

 <li><strong>What is the priority inversion problem? Does this problem occur if round-robin scheduling is used instead of priority scheduling? Discuss. (2 points) </strong></li>

</ol>

Priority inversion problem will not occur in Round-Robin. Due to the fact that RR schedules processes in a way that one process can only use a certain amount of time before it is forced to pop out and wait for the next process.




<ol start="8">

 <li><strong>Does Peterson’s solution to the mutual exclusion problem work when process scheduling is preemptive? How about when it is non-preemptive? (2 points) </strong></li>

</ol>

Peterson’s solution was designed to work when the scheduling is preemptive. When the scheduling is non-preemptive, it may not work. It will loop through forever and never gets release.
















<ol start="9">

 <li><strong>Consider the following set of processes, with the length of the CPU burst time given in milliseconds: </strong></li>

</ol>

<strong>Process       Burst-Time        Priority </strong>

<strong>P1                    6                      3 </strong>

<strong>P2                    1                      1 </strong>

<strong>P3                    2                      5 </strong>

<strong>P4                    3                      4 </strong>

<strong>P5                    5                      2 </strong>

<strong>The processes are assumed to have arrived in the order P1, P2, P3, P4, P5, all at time 0. </strong>

<ul>

 <li><strong>Draw four Gantt charts illustrating the execution of these processes using FCFS, SJF, a nonpreemptive priority (a smaller priority number implies a higher priority), and RR (quantum = 1) scheduling. </strong></li>

</ul>




<ul>

 <li><strong>What is the turnaround time of each process for each of the scheduling algorithms in part (a)?</strong></li>

</ul>




<table>

 <tbody>

  <tr>

   <td width="90">PROCESS</td>

   <td width="60">FIFO</td>

   <td width="60">SJF</td>

   <td width="150">NONPREEMPTIVE</td>

   <td width="66">RR</td>

  </tr>

  <tr>

   <td width="90">P1</td>

   <td width="60">6</td>

   <td width="60">17</td>

   <td width="150">12</td>

   <td width="66">17</td>

  </tr>

  <tr>

   <td width="90">P2</td>

   <td width="60">7</td>

   <td width="60">1</td>

   <td width="150">1</td>

   <td width="66">2</td>

  </tr>

  <tr>

   <td width="90">P3</td>

   <td width="60">9</td>

   <td width="60">3</td>

   <td width="150">17</td>

   <td width="66">7</td>

  </tr>

  <tr>

   <td width="90">P4</td>

   <td width="60">12</td>

   <td width="60">6</td>

   <td width="150">15</td>

   <td width="66">11</td>

  </tr>

  <tr>

   <td width="90">P5</td>

   <td width="60">17</td>

   <td width="60">11</td>

   <td width="150">6</td>

   <td width="66">16</td>

  </tr>

  <tr>

   <td width="90">TOTAL</td>

   <td width="60">51</td>

   <td width="60">38</td>

   <td width="150">51</td>

   <td width="66">53</td>

  </tr>

 </tbody>

</table>










<ul>

 <li><strong>What is the waiting time of each process for each of the scheduling algorithm s in part (a)? </strong></li>

</ul>

<table width="431">

 <tbody>

  <tr>

   <td width="91">PROCESS</td>

   <td width="67">FIFO</td>

   <td width="63">SJF</td>

   <td width="148">NONPREEMPTIVE</td>

   <td width="62">RR</td>

  </tr>

  <tr>

   <td width="91">P1</td>

   <td width="67">0</td>

   <td width="63">11</td>

   <td width="148">6</td>

   <td width="62">11</td>

  </tr>

  <tr>

   <td width="91">P2</td>

   <td width="67">6</td>

   <td width="63">0</td>

   <td width="148">0</td>

   <td width="62">1</td>

  </tr>

  <tr>

   <td width="91">P3</td>

   <td width="67">7</td>

   <td width="63">1</td>

   <td width="148">15</td>

   <td width="62">5</td>

  </tr>

  <tr>

   <td width="91">P4</td>

   <td width="67">9</td>

   <td width="63">3</td>

   <td width="148">12</td>

   <td width="62">8</td>

  </tr>

  <tr>

   <td width="91">P5</td>

   <td width="67">12</td>

   <td width="63">6</td>

   <td width="148">1</td>

   <td width="62">11</td>

  </tr>

  <tr>

   <td width="91">TOTAL</td>

   <td width="67">34</td>

   <td width="63">21</td>

   <td width="148">34</td>

   <td width="62">36</td>

  </tr>

  <tr>

   <td width="91">AVERAGE</td>

   <td width="67">6.8</td>

   <td width="63">4.2</td>

   <td width="148">6.8</td>

   <td width="62">7.2</td>

  </tr>

 </tbody>

</table>










<ul>

 <li><strong>Which of the schedules in part a result in the minimal average waiting time (over all processes)? (5 points) </strong></li>

</ul>




Shortest Job First has the minimal average waiting time.










<ol start="10">

 <li><strong>The aging algorithm with a = 1/2 is being used to predict run times. The previous four runs, from oldest to most recent, are 40, 20, 40, and 15 msec. What is the prediction of the next time? </strong></li>

</ol>




= (((40 + 20) / 2 + 40) / 2 + 15) / 2

= ((30 + 40) / 2 + 15) /2

= (35 + 15) / 2

= 25




<ol start="11">

 <li><strong>12) Explain what a multi-level feedback scheduler is and why it approximates SRTF.</strong><strong>True </strong><strong>or </strong><strong>False </strong><strong>(also give an explanation for your choice): If a user knows the length of a CPU time-slice and can determine precisely how long his process has been running, then he can cheat a multi-level feedback scheduler. (2 points) </strong></li>

</ol>




Multilevel feedback queue-scheduling algorithm allows a process to move between queues. It uses many ready queues and associate a different priority with each queue. I think it is <strong>True</strong> that if a user knows the length of a CPU time-slice and can determine precisely how long his process has been running, then he can cheat a multi-level feedback scheduler. User can just execute an I/O request that would allow for the process to get more time that it is supposed to.










<ol start="12">

 <li><strong>Consider a system consisting of processes </strong><strong><em>P</em></strong><strong>1</strong><strong>, </strong><strong><em>P</em></strong><strong>2</strong><strong>, …, </strong><strong><em>P</em></strong><strong><em>n</em></strong><strong>, each of which has a unique priority number. Write the pseudo-code of a monitor that allocates three identical line printers to these processes, using the priority numbers for deciding the order of allocation. (5 points) </strong><strong>Start with the following and populate the two functions request_printer() and release_printer(): </strong></li>

</ol>

<strong> </strong>

<strong>monitor printers </strong><strong><em>{</em></strong><strong>int num_avail = 3;int waiting_processes[MAX PROCS]; int num_waiting;condition c; </strong>

<strong>void request_printer(int proc_number) </strong><strong><em>{ </em></strong>

<strong><em>} </em></strong>

<strong>void release_printer() </strong><strong><em>{ </em></strong>

<strong><em>} } </em></strong>

<em> </em>

Solution:

monitor printers <em>{</em>

<em></em>int num_avail = 3;int waiting_processes[MAX PROCS];

int num_waiting;condition c;

void request_printer(int proc_number) <em>{ </em>

<em> </em>

<em>if (num_avail less than o) {</em>

<em>num_avail – -;</em>

<em>return;</em>

<em>}</em>

waiting_processes[num waiting] = proc_number

num_waiting ++;

while(num_avail == 0){

condition c.wait();




wait process[0] = wait processes[num waiting – 1]

num waiting–;

sort waiting processes;

num available –;

}




<em> </em>




<em>} </em>

void release_printer() <em>{ </em>

<em>num avail ++;</em>

<em>condition c.broadcast();</em>

<em>} } </em>






















<em> </em>

<em> </em>










<em> </em>











