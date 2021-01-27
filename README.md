# Data Wrangling
In-person class challenge for data wrangling.

## Assigned play:

I am from section 01, group B and my number is 3, so I was assigned the play, 'The Comedy of Errors' by Shakespeare.

```
http://shakespeare.mit.edu/comedy_errors/full.html
```

## My Speakers:

1. Speaker 1 - LUCIANA

2. Speaker 2 - ADRIANA

## Question asked:

**Who speaks more? Speaker 1 or speaker 2?**

## Commands used (BASH):

1. I have used curl command for storingand sorting text data in an input file called "ac-input.txt" from the URL.

```
$ curl "http://shakespeare.mit.edu/comedy_errors/full.html" | sed 's/<\/*[^>]*>//g' > "ac-input.txt"
```

2. I have used the curl command for displaying 'LUCIANA' from the input text file.

```
$ grep 'LUCIANA' ac-input.txt
```

3. Then, I used the following command for counting the number of times 'LUCIANA' appears.

```
$ grep 'LUCIANA' ac-input.txt -c
50
```

4. Similarly, I used the same command for counting 'ADRIANA'.

```
$ grep 'ADRIANA' ac-input.txt -c
84
```

5. I have then stored these values in two different output text files.

```
$ grep 'ADRIANA' ac-input.txt -c > "ac-output.txt"
$ grep 'LUCIANA' ac-input.txt -c > "ac-output2.txt"
$ grep 'LUCIANA' ac-input.txt -c > "ac-output-luciana.txt"
$ grep 'ADRIANA' ac-input.txt -c > "ac-output-adriana.txt"
```
*Note: I have deleted ac-output.txt and ac-output2.txt*

## Link to the input file:

(after data sorting)
[ac-input.txt](https://github.com/annie0sc/ac-wrangle/blob/main/ac-input.txt)

## Links to the count:

1. [LUCIANA: 50](https://github.com/annie0sc/ac-wrangle/blob/main/ac-output-luciana.txt)

2. [ADRIANA: 84](https://github.com/annie0sc/ac-wrangle/blob/main/ac-output-adriana.txt)

# Answer:

*Clearly, Andriana likes to speak more than Luciana ;)*

### Screenshot:

![](https://github.com/annie0sc/ac-wrangle/blob/main/Screenshot%20(104).png)