# topic
In this article, I will teach you how to use Python modules to scrawl youtube transcript.
We can automatically get the transcript with less effort if we use this module.

# NOTE
1. check the module "youtube_transcript_api" can work as well.

# Import
1. To use the module "youtube_transcript_api", import the module by typing
from youtube_transcript_api import YouTubeTranscriptApi

# Use
It is easy to use.

step 1:
Copy the url.

step 2:
Paste the url and then put it into the variable as string type. 
I called the variable -- video_url.
Type the such following code in you IDE.
video_url='https://www.youtube.com/watch?v=JMOp5n3YgLA'

step 3:
Split the string and fetch the letters after first '=' and put it into the variable as string type.
I called the variable -- video_id.


Type the such following code in you IDE.
video_id=video_url.split('=')[1]

step 4:
Feed the video_id and get the information about youtube transcript then put it into a variable.
I called the variable -- video_info.

Type the such following code in you IDE.
video_info=YouTubeTranscriptApi.get_transcript(video_id)

# Complaint
I really want to complain about the website.
https://pypi.org/project/youtube-transcript-api/0.4.4/#api
It does NOT tell me what the variable video_id should be.
I found the solution for a while. 
And I really appreicate to the YT video.
https://www.youtube.com/watch?v=3V-MJhJvRWg&t=2s
I found the solution in this video.


# Example
## Example Code

from youtube_transcript_api import YouTubeTranscriptApi

video_url='https://www.youtube.com/watch?v=JMOp5n3YgLA'
video_id=video_url.split('=')[1]
print(video_id)
video_info=YouTubeTranscriptApi.get_transcript(video_id)
print('-----------------------')
for v_info in video_info:
    print(v_info)

## Example demo
The demo and tutorial of the module:
https://www.youtube.com/watch?v=d8NyUg61ws8


## Example intro 
Scrawl the youtube transcript of the following link.
https://www.youtube.com/watch?v=JMOp5n3YgLA


## Example Output
JMOp5n3YgLA
-----------------------
{'text': 'hello everyone', 'start': 0.359, 'duration': 3.421}
{'text': "in this video we're going to be solving", 'start': 1.92, 'duration': 5.04}
{'text': 'a quintic equation and this is not going', 'start': 3.78, 'duration': 5.279}
{'text': "to be my first quintic we've done", 'start': 6.96, 'duration': 4.86}
{'text': 'quintix before and by the way this is a', 'start': 9.059, 'duration': 5.761}
{'text': 'video response to Black pen red pen', 'start': 11.82, 'duration': 5.4}
{'text': "I'm pretty sure you know him I'm also", 'start': 14.82, 'duration': 4.62}
{'text': 'going to share the link here for his', 'start': 17.22, 'duration': 4.2}
{'text': 'video so you can take a look all right', 'start': 19.44, 'duration': 4.14}
{'text': "we have this quintic equation it's", 'start': 21.42, 'duration': 4.56}
{'text': "missing a lot of terms that's why it's a", 'start': 23.58, 'duration': 4.859}
{'text': "little easier to factor so we're going", 'start': 25.98, 'duration': 3.9}
{'text': 'to look at the solution', 'start': 28.439, 'duration': 5.28}
{'text': "and then we're going to be looking at", 'start': 29.88, 'duration': 8.1}
{'text': "the graph all right so let's see how we", 'start': 33.719, 'duration': 6.061}
{'text': 'can handle this', 'start': 37.98, 'duration': 5.099}
{'text': "so I'm going to manipulate this x to the", 'start': 39.78, 'duration': 4.74}
{'text': "fifth term a little bit so I'm going to", 'start': 43.079, 'duration': 4.621}
{'text': 'write this as x to the fifth minus x', 'start': 44.52, 'duration': 6.84}
{'text': 'squared plus x squared plus x to the', 'start': 47.7, 'duration': 4.74}
{'text': 'fourth', 'start': 51.36, 'duration': 3.719}
{'text': 'plus one equals zero now why am I doing', 'start': 52.44, 'duration': 4.799}
{'text': 'this you might be questioning where on', 'start': 55.079, 'duration': 4.441}
{'text': 'Earth does this minus x squared come', 'start': 57.239, 'duration': 4.381}
{'text': 'from first of all it works right if you', 'start': 59.52, 'duration': 4.92}
{'text': 'subtracted a term and add the same one', 'start': 61.62, 'duration': 5.16}
{'text': 'totally fine but why is it x squared', 'start': 64.44, 'duration': 5.16}
{'text': 'okay couple reasons first of all it', 'start': 66.78, 'duration': 5.4}
{'text': 'makes this expression factorable by', 'start': 69.6, 'duration': 6.0}
{'text': 'grouping and these two groups have a', 'start': 72.18, 'duration': 6.54}
{'text': "common factor why let's see why so we'll", 'start': 75.6, 'duration': 5.159}
{'text': "take out x squared here it's going to be", 'start': 78.72, 'duration': 5.759}
{'text': 'X cubed minus 1. and then this term here', 'start': 80.759, 'duration': 5.22}
{'text': "I'm going to leave that alone for now", 'start': 84.479, 'duration': 3.481}
{'text': "and then I'll Factor it separately and", 'start': 85.979, 'duration': 4.741}
{'text': 'just copy and paste it here okay so', 'start': 87.96, 'duration': 4.86}
{'text': "let's take care of this first of all X", 'start': 90.72, 'duration': 5.039}
{'text': 'cubed minus 1 is difference of two cubes', 'start': 92.82, 'duration': 6.9}
{'text': 'so I can Factor it as x minus 1 times x', 'start': 95.759, 'duration': 6.18}
{'text': 'squared plus X plus one', 'start': 99.72, 'duration': 4.14}
{'text': "and now let's go ahead and focus on this", 'start': 101.939, 'duration': 3.421}
{'text': "and then we'll go ahead and paste it", 'start': 103.86, 'duration': 4.02}
{'text': 'over there so how do you factor x to the', 'start': 105.36, 'duration': 6.18}
{'text': 'fourth plus x squared plus one okay so', 'start': 107.88, 'duration': 6.84}
{'text': 'this can be completed to a square so in', 'start': 111.54, 'duration': 5.759}
{'text': 'other words if I add x squared to this', 'start': 114.72, 'duration': 4.439}
{'text': 'it becomes x to the fourth plus two x', 'start': 117.299, 'duration': 3.541}
{'text': 'squared plus one which is a perfect', 'start': 119.159, 'duration': 4.14}
{'text': 'square but I also need to subtract x', 'start': 120.84, 'duration': 5.879}
{'text': 'squared to balanced equation make sense', 'start': 123.299, 'duration': 6.66}
{'text': '2x squared minus x squared is equal to x', 'start': 126.719, 'duration': 5.701}
{'text': "squared so we're all good but I did this", 'start': 129.959, 'duration': 5.341}
{'text': 'because this is a perfect square and', 'start': 132.42, 'duration': 5.16}
{'text': 'that is perfect so I can write it as x', 'start': 135.3, 'duration': 6.6}
{'text': 'squared plus 1 squared minus x squared', 'start': 137.58, 'duration': 5.64}
{'text': "you don't have to put the X in", 'start': 141.9, 'duration': 2.52}
{'text': 'parenthesis but I just wanted to', 'start': 143.22, 'duration': 3.54}
{'text': 'emphasize the difference of two squares', 'start': 144.42, 'duration': 3.959}
{'text': 'formula here so you can see the pattern', 'start': 146.76, 'duration': 4.14}
{'text': 'and the pattern says what a squared', 'start': 148.379, 'duration': 5.821}
{'text': 'minus B squared is a plus b times a', 'start': 150.9, 'duration': 5.22}
{'text': 'minus B this is one of the most', 'start': 154.2, 'duration': 4.44}
{'text': 'important identities in math I think you', 'start': 156.12, 'duration': 4.68}
{'text': 'should all know this so now we can', 'start': 158.64, 'duration': 4.08}
{'text': 'Factor it as x squared plus plus 1 plus', 'start': 160.8, 'duration': 4.019}
{'text': 'X but I can write it as x squared plus X', 'start': 162.72, 'duration': 4.64}
{'text': 'Plus 1 because we should always write', 'start': 164.819, 'duration': 5.161}
{'text': 'polynomials in standard form right and', 'start': 167.36, 'duration': 3.82}
{'text': 'then the other factor is going to be x', 'start': 169.98, 'duration': 2.94}
{'text': 'squared plus 1 minus X but I can write', 'start': 171.18, 'duration': 4.8}
{'text': 'it as x squared minus X Plus 1. great so', 'start': 172.92, 'duration': 4.56}
{'text': "we're going to go ahead and take this", 'start': 175.98, 'duration': 4.979}
{'text': 'expression and paste it over here so we', 'start': 177.48, 'duration': 4.86}
{'text': 'need to add', 'start': 180.959, 'duration': 4.201}
{'text': "this one let's go ahead and do it now", 'start': 182.34, 'duration': 5.1}
{'text': "so I'm not going to need the equal sign", 'start': 185.16, 'duration': 4.88}
{'text': 'so let me go ahead and cut it like this', 'start': 187.44, 'duration': 6.06}
{'text': 'and bring it over here is it going to', 'start': 190.04, 'duration': 4.6}
{'text': 'fit hopefully', 'start': 193.5, 'duration': 2.879}
{'text': 'okay', 'start': 194.64, 'duration': 4.26}
{'text': "I think it's gonna work right well the", 'start': 196.379, 'duration': 3.901}
{'text': 'parentheses are kind of out of bounds', 'start': 198.9, 'duration': 3.059}
{'text': "but hopefully it'll work okay I can do", 'start': 200.28, 'duration': 5.28}
{'text': 'the following uh let me do this and then', 'start': 201.959, 'duration': 6.181}
{'text': "I'm gonna move the whole thing", 'start': 205.56, 'duration': 4.259}
{'text': "so hopefully it'll be better okay here", 'start': 208.14, 'duration': 4.62}
{'text': "we go so now we've taken care of this", 'start': 209.819, 'duration': 5.161}
{'text': 'and I can get rid of this part', 'start': 212.76, 'duration': 5.3}
{'text': "I don't need it anymore", 'start': 214.98, 'duration': 3.08}
{'text': 'now', 'start': 218.4, 'duration': 2.94}
{'text': 'what are we going to do with this we', 'start': 219.54, 'duration': 3.419}
{'text': 'have a common factor like I said earlier', 'start': 221.34, 'duration': 4.02}
{'text': 'this is not factorable because x squared', 'start': 222.959, 'duration': 5.221}
{'text': 'plus X Plus 1 is a common factor I can', 'start': 225.36, 'duration': 4.799}
{'text': 'take it out', 'start': 228.18, 'duration': 4.5}
{'text': 'and then the other factors are going to', 'start': 230.159, 'duration': 4.621}
{'text': 'be x squared times x minus 1. I can', 'start': 232.68, 'duration': 4.68}
{'text': 'definitely distribute right and write it', 'start': 234.78, 'duration': 5.7}
{'text': 'as X cubed minus x squared', 'start': 237.36, 'duration': 4.26}
{'text': 'and then', 'start': 240.48, 'duration': 4.08}
{'text': 'plus plus this is the plus sign right', 'start': 241.62, 'duration': 5.22}
{'text': "here and now we're here", 'start': 244.56, 'duration': 5.7}
{'text': "x squared minus X plus 1. that's kind of", 'start': 246.84, 'duration': 6.0}
{'text': "like a long you know Factor but don't", 'start': 250.26, 'duration': 4.619}
{'text': "worry it's going to simplify because x", 'start': 252.84, 'duration': 4.799}
{'text': 'squared cancels out and we end up with x', 'start': 254.879, 'duration': 5.42}
{'text': 'squared plus X plus one', 'start': 257.639, 'duration': 7.921}
{'text': 'multiply by x cubed minus X plus one', 'start': 260.299, 'duration': 9.521}
{'text': 'equals zero and our equation is factored', 'start': 265.56, 'duration': 6.419}
{'text': 'so this is just another approach to', 'start': 269.82, 'duration': 3.72}
{'text': 'factor it obviously there is more than', 'start': 271.979, 'duration': 4.381}
{'text': "one way to do it now let's solve the", 'start': 273.54, 'duration': 3.9}
{'text': 'equation', 'start': 276.36, 'duration': 3.3}
{'text': "the first one is easy because it's", 'start': 277.44, 'duration': 4.08}
{'text': "quadratic let's go ahead and write the", 'start': 279.66, 'duration': 4.62}
{'text': 'roots by quadratic formula negative B', 'start': 281.52, 'duration': 5.459}
{'text': 'plus minus the square root of B squared', 'start': 284.28, 'duration': 4.979}
{'text': "which is 1 minus four that's going to be", 'start': 286.979, 'duration': 3.901}
{'text': 'negative 3 but I can write it as square', 'start': 289.259, 'duration': 3.841}
{'text': 'root of 3 I remember complex numbers', 'start': 290.88, 'duration': 3.72}
{'text': "we've done some complex number videos", 'start': 293.1, 'duration': 4.2}
{'text': 'recently divide by two so those are the', 'start': 294.6, 'duration': 4.86}
{'text': 'solutions to the quadratic how about the', 'start': 297.3, 'duration': 6.0}
{'text': "cubic we have a cubic formula but let's", 'start': 299.46, 'duration': 5.76}
{'text': 'go ahead and go through the process yes', 'start': 303.3, 'duration': 3.54}
{'text': "you can memorize it but I don't", 'start': 305.22, 'duration': 4.02}
{'text': 'recommend uh you definitely can but if', 'start': 306.84, 'duration': 4.799}
{'text': "you have can refer to your notes let's", 'start': 309.24, 'duration': 3.78}
{'text': "say you're taking a test and you're", 'start': 311.639, 'duration': 3.301}
{'text': 'allowed to use your notes obviously you', 'start': 313.02, 'duration': 3.66}
{'text': "can do that so here's what I'm going to", 'start': 314.94, 'duration': 4.199}
{'text': "do I'm going to set this equal to 0", 'start': 316.68, 'duration': 4.459}
{'text': 'first', 'start': 319.139, 'duration': 5.701}
{'text': 'and then isolate the constant', 'start': 321.139, 'duration': 6.28}
{'text': "and then now we're gonna", 'start': 324.84, 'duration': 4.38}
{'text': 'turn this into', 'start': 327.419, 'duration': 4.201}
{'text': "an identity that we can use so here's", 'start': 329.22, 'duration': 4.02}
{'text': "here's our cubic let's we're going to", 'start': 331.62, 'duration': 3.0}
{'text': 'solve that equation now but let me go', 'start': 333.24, 'duration': 3.72}
{'text': 'ahead and rewrite that identity we just', 'start': 334.62, 'duration': 3.6}
{'text': 'recently used right I think it was', 'start': 336.96, 'duration': 2.28}
{'text': 'yesterday', 'start': 338.22, 'duration': 3.66}
{'text': 'uh we talked about this right so a plus', 'start': 339.24, 'duration': 8.459}
{'text': 'b cubed minus 3 a b times a plus b', 'start': 341.88, 'duration': 9.06}
{'text': 'equals a cubed plus B Cubed', 'start': 347.699, 'duration': 4.5}
{'text': 'now', 'start': 350.94, 'duration': 4.319}
{'text': "we're going to go ahead and we're going", 'start': 352.199, 'duration': 4.581}
{'text': 'to go ahead and', 'start': 355.259, 'duration': 4.981}
{'text': "associate these two equations how we're", 'start': 356.78, 'duration': 6.88}
{'text': 'going to call this x and x so now 3ab', 'start': 360.24, 'duration': 5.459}
{'text': 'becomes the coefficient of x but the', 'start': 363.66, 'duration': 4.68}
{'text': 'coefficient of x is negative one here', 'start': 365.699, 'duration': 5.881}
{'text': "it's negative 3 a b so 3ab must equal 1", 'start': 368.34, 'duration': 5.699}
{'text': 'and the constant term AQ plus B Cubed', 'start': 371.58, 'duration': 5.16}
{'text': 'must equal negative one great so we got', 'start': 374.039, 'duration': 7.681}
{'text': 'a system a b equals 1 3 because 3 a b is', 'start': 376.74, 'duration': 8.04}
{'text': '1 positive one remember and a cubed plus', 'start': 381.72, 'duration': 5.94}
{'text': "B Cubed is negative one we can't find a", 'start': 384.78, 'duration': 5.22}
{'text': 'and b by guessing because they are very', 'start': 387.66, 'duration': 4.5}
{'text': "very irrational but let's go ahead and", 'start': 390.0, 'duration': 5.1}
{'text': "find them because uh easy it's easy to", 'start': 392.16, 'duration': 7.28}
{'text': "find so let's cue both sides here", 'start': 395.1, 'duration': 4.34}
{'text': "then we're gonna go ahead and isolate B", 'start': 400.86, 'duration': 6.54}
{'text': 'Cubed write it as negative a cubed minus', 'start': 404.28, 'duration': 5.16}
{'text': "one and we're going to go ahead and", 'start': 407.4, 'duration': 4.56}
{'text': "substitute that here that's how the", 'start': 409.44, 'duration': 4.979}
{'text': "cubic formula Works let's do it a cubed", 'start': 411.96, 'duration': 4.98}
{'text': 'times B Cubed which is negative a cubed', 'start': 414.419, 'duration': 7.261}
{'text': 'minus 1 equals 0 not 0 1 over 27. uh I', 'start': 416.94, 'duration': 5.94}
{'text': 'think the problem that we did yesterday', 'start': 421.68, 'duration': 3.239}
{'text': "I didn't complete the first solution", 'start': 422.88, 'duration': 3.84}
{'text': 'because that was kind of painful but', 'start': 424.919, 'duration': 2.761}
{'text': "this time we're going to do it", 'start': 426.72, 'duration': 3.78}
{'text': 'completely so now uh if you distribute', 'start': 427.68, 'duration': 4.62}
{'text': 'and put everything on the right hand', 'start': 430.5, 'duration': 4.44}
{'text': 'side you get a to the 6 plus a cubed', 'start': 432.3, 'duration': 6.6}
{'text': 'plus 1 over 27 equals zero and if you', 'start': 434.94, 'duration': 6.3}
{'text': 'set a cubed equal to C', 'start': 438.9, 'duration': 4.98}
{'text': 'hopefully you see what I see you get c', 'start': 441.24, 'duration': 6.54}
{'text': 'squared plus C plus 1 over 27 equals', 'start': 443.88, 'duration': 5.879}
{'text': 'zero and guess what this is a quadratic', 'start': 447.78, 'duration': 4.319}
{'text': 'so while solving the cubic after you do', 'start': 449.759, 'duration': 5.22}
{'text': 'all these Transformations uh you do get', 'start': 452.099, 'duration': 4.981}
{'text': 'a quadratic same thing with the cortic', 'start': 454.979, 'duration': 4.62}
{'text': 'if you play around with the cortic you', 'start': 457.08, 'duration': 4.5}
{'text': 'get a cubic and then you can solve that', 'start': 459.599, 'duration': 3.961}
{'text': 'cubic all right', 'start': 461.58, 'duration': 4.8}
{'text': "so let's see what we can do easy right", 'start': 463.56, 'duration': 4.62}
{'text': "and I'm also going to show you what tool", 'start': 466.38, 'duration': 4.14}
{'text': 'from alpha gave us as Solutions but let', 'start': 468.18, 'duration': 3.66}
{'text': 'me go ahead and work this out first', 'start': 470.52, 'duration': 4.579}
{'text': 'negative 1 plus minus square root of B', 'start': 471.84, 'duration': 7.579}
{'text': "squared minus 4AC that's 4 over 27 over", 'start': 475.099, 'duration': 6.94}
{'text': "2. and if you simplify this you're going", 'start': 479.419, 'duration': 4.84}
{'text': 'to get the following 9 which is kind of', 'start': 482.039, 'duration': 4.44}
{'text': 'surprising right plus minus square root', 'start': 484.259, 'duration': 6.78}
{'text': 'of 69 divided by 8. awesome this this is', 'start': 486.479, 'duration': 6.78}
{'text': 'those are the C values and C is equal to', 'start': 491.039, 'duration': 4.201}
{'text': 'a cubed remember so keep that in mind', 'start': 493.259, 'duration': 4.861}
{'text': "because we're going to work it out so", 'start': 495.24, 'duration': 4.739}
{'text': 'let me go ahead and show you what from', 'start': 498.12, 'duration': 5.699}
{'text': 'alpha gave me for the real solutions and', 'start': 499.979, 'duration': 4.921}
{'text': 'I think we already talked about the', 'start': 503.819, 'duration': 2.94}
{'text': 'complex Solutions right', 'start': 504.9, 'duration': 5.16}
{'text': "so that's how it gave it to us a little", 'start': 506.759, 'duration': 5.101}
{'text': 'bit of manipulation is required but', 'start': 510.06, 'duration': 6.539}
{'text': "anyways easy okay so let's go ahead and", 'start': 511.86, 'duration': 7.679}
{'text': 'finish this up so we got the a cubed so', 'start': 516.599, 'duration': 5.641}
{'text': 'if you take the positive value you can', 'start': 519.539, 'duration': 5.461}
{'text': 'find the a from here which is going to', 'start': 522.24, 'duration': 5.76}
{'text': 'be cube root of 9 plus square root of 69', 'start': 525.0, 'duration': 6.12}
{'text': 'over 8. and B can be the other one and', 'start': 528.0, 'duration': 5.1}
{'text': "they can switch around two but that's", 'start': 531.12, 'duration': 3.74}
{'text': 'not a ninth root note', 'start': 533.1, 'duration': 4.5}
{'text': "because it doesn't matter", 'start': 534.86, 'duration': 6.4}
{'text': 'remember X is equal to a plus b', 'start': 537.6, 'duration': 6.359}
{'text': "and I think it's not X it's Y is it X", 'start': 541.26, 'duration': 6.18}
{'text': 'okay x x equal to a plus b so x equals', 'start': 543.959, 'duration': 5.761}
{'text': 'the sum of these two', 'start': 547.44, 'duration': 5.64}
{'text': 'nice quantities', 'start': 549.72, 'duration': 5.4}
{'text': "it's this one", 'start': 553.08, 'duration': 3.66}
{'text': 'Plus', 'start': 555.12, 'duration': 3.36}
{'text': 'this one', 'start': 556.74, 'duration': 4.68}
{'text': "how nice right okay okay so that's the", 'start': 558.48, 'duration': 5.039}
{'text': "solution that we get from here and let's", 'start': 561.42, 'duration': 5.82}
{'text': 'go ahead and take a look at', 'start': 563.519, 'duration': 7.021}
{'text': "the graph and we'll finish up so that's", 'start': 567.24, 'duration': 4.68}
{'text': 'the real solution again one more time', 'start': 570.54, 'duration': 3.54}
{'text': "and here's the graph of x to the fifth", 'start': 571.92, 'duration': 4.859}
{'text': 'plus x to the fourth plus one equals', 'start': 574.08, 'duration': 4.8}
{'text': 'zero remember we have the quadratic and', 'start': 576.779, 'duration': 3.961}
{'text': 'a cubic the quadratic', 'start': 578.88, 'duration': 4.019}
{'text': "didn't have any real solutions and the", 'start': 580.74, 'duration': 5.279}
{'text': 'cubic only has one real solution if you', 'start': 582.899, 'duration': 4.56}
{'text': "want to find the other one Ah that's", 'start': 586.019, 'duration': 4.861}
{'text': 'very painful you can do it but', 'start': 587.459, 'duration': 5.041}
{'text': 'this brings us to the end of this video', 'start': 590.88, 'duration': 2.82}
{'text': 'thanks for watching I hope you enjoyed', 'start': 592.5, 'duration': 3.06}
{'text': "it please let me know don't forget to", 'start': 593.7, 'duration': 3.42}
{'text': "comment like And subscribe I'll see you", 'start': 595.56, 'duration': 3.48}
{'text': 'tomorrow with another video Until then', 'start': 597.12, 'duration': 7.159}
{'text': 'be safe take care and bye bye', 'start': 599.04, 'duration': 5.239}
