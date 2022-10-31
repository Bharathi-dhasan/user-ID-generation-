# user-ID-generation-
Joseph&#39;s team has been assigned the task of creating user-ids for all participants of an
online gaming competiton. Joseph has designed a process for generating the user-id
using the participant&#39;s First_name,Last_Name,PIN code and a number N. The process
defined by Joseph is as below-
STEP 1-Compare the lengths of FIRST_Name and Last_name of the participant. The one
that is shorter will be called &quot;Smaller Name&quot; and the one that is longer will be called the
&quot;Longer name&quot;. If the both First_name and Last_name are of equal length, then the
name that appears earlier in alphabetical order will be &quot;Smaller Name&quot; and the name
that appears later in alphabetical order will be called the &quot;Longer name&quot;.
STEP 2:The user-id should be generated as below-First Letter of the longer name+ Entire
word of the smaller name+ digit at position N in the PIN when traversing the PIN from
Left to right+ Digit at position N in the PIN when traversing the PIN from right to left.
STEP 3: Toggle the Alphabets of the user-id generated in step-2.i.e.upper-case
alphabets should become lower-case and lower-case should become upper-case
Let us see few Examples.
EXAMPLE-1: If the participant&#39;s details are as below-
First_Name =Rajiv
LAst_Name =Roy
PIN=560037
N=6
STEP-1:Length of Last_name is less than the Length of First_name, so that Smaller name
is&quot;Roy&quot; and the longer name is &quot;Rajiv&quot;
STEP-2:The user-id will be=First Letter of the longer name+Entire word of the smaller
name+digit at position N in the PIN when traversing the PIN from left to right+Digit at
position N in the PIN when traversing the PIN from right to left
= First Letter of &quot;Rajiv&quot; + Entire word of &quot; Roy &quot;+6th didgit of PIN from left+6th digit of
PIN from right.
=R+Roy+7+5
therefore,user-id=RRoy75
STEP-3:Toggle the alphabets in the user-id.So,user-id=rrOY75
EXAMPLE-2: If the participant&#39;s details are as below-
First_Name =Manoj
LAst_Name =Kumar
PIN=561327
N=2

STEP-1: Length of First_name is equal to the Length of Last_name .Alphabetially
,&quot;Kumar&quot; appears earlier than &quot;Manoj&quot;(by comparing alphabetic positions of &#39;k&#39; and &#39;M&#39;
so that Smaller name is&quot;Kumar&quot; and the longer name is &quot;Manoj&quot;
STEP-2:The user-id will be=First Letter of the longer name+Entire word of the smaller
name+digit at position N in the PIN when traversing the PIN from left to right+Digit at
position N in the PIN when traversing the PIN from right to left
= First Letter of &quot;Manoj&quot; + Entire word of &quot; Kumar &quot;+2th didgit of PIN from left+2th digit
of PIN from right.
=M+Kumar+6+2
therefore, user-id=MKumar62
STEP-3:Toggle the alphabets in the user-id.So,user-id=mkUMAR62
EXAMPLE-3: If the participant&#39;s details are as below-
First_Name =Kumud
LAst_Name =Kumar
PIN=561327
N=2
STEP-1: Length of First_name is equal to the Length of Last_name .Alphabetically
,&quot;Kumar&quot; appears earlier than &quot;Kumud&quot;(by comparing alphabetic positions of &#39;A&#39; and &#39;U&#39;
so that Smaller name is &quot;Kumar&quot; and the longer name is &quot;KUMUD&quot;
STEP-2:The user-id will be=First Letter of the longer name+ Entire word of the smaller
name+ digit at position N in the PIN when traversing the PIN from left to right+ Digit at
position N in the PIN when traversing the PIN from right to left
= First Letter of &quot;Kumud&quot; + Entire word of &quot; Kumar &quot;+2th digit of PIN from left+2th digit
of PIN from right.
=K+Kumar+6+2
therefore, user-id=KKumar62
STEP-3:Toggle the alphabets in the user-id. So, user-id=kkUMAR62
You are part of Joseph&#39;s team and he has asked you to write a program(method) to
generate the participants user-id using the above rules.
The prototype of the method(function) should be as below-
public static void useridgeneration(String input1, String input2,int input3,int input4)
where,
 is the First_Name
 is the Last_Name
 is the PIN
 is the number N
The method(function) should do the processing as per rules explained above and should
assign the generated user-id to the member variable Output1
