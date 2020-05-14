# Shell Data Processing

When creating a project, I started by opening my folder creaeted 44517.  This is for the Big Data Cours that I am currently enrolled in and follows the format that I use for many other courses. 

## Project Creation
One of the first exercises was to create a project by navigating to the 44517 folder.
- The folder was opened in a powershell window by choosing the context menu option "Open Powershell window here as administrator."

- From that prompt, I created a new directory called "shell-data-processing" by running the following:

``` mkdir shell-data-processing ```

- Then I changed directory to "shell-data-processing" with the cd command:

``` cd shell-data-processing ```

- Using the new item command, ni, I created a new file called "README.md"

``` ni README.md ```

- By recalling the previous command using the up arrow, I modified the command and created a new file called ".gitignore"  The file was sourced from the "big-data-developers" project

``` ni .gitignore ```

- To list the files in the directory, you can use each of the following commands.

``` ls ```  
``` dir ```  
``` gci ```  

## Curl "Not rigging a vote this time"

After looking around on Wikipedia a bit, I found an entry on [Vincent van Gogh]https://en.wikipedia.org/wiki/Vincent_van_Gogh

I then ran the curl command to output the previous link output to a file called data.txt

```curl https://en.wikipedia.org/wiki/Vincent_van_Gogh -O data.txt```

## Bash Commands 'Bourne Again Shell'

The to purch space characters into an ASCII line feed character I am running the following command

```tr ' ' '\12' < data.txt```

Next I sorted the data file with the following command:

```tr ' ' '\12' < data.txt | sort```

Then I sorted the output to a uniq-c to count each instance of words

```tr ' ' '\12' < data.txt | sort | uniq -c```

Next I reduced the output using the sort with the -nr flag

```tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr```

And I redirect the output from data.txt into result.txt

```tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr > result.txt```

I have been hitting the up arrow to repeat and modify the previous commands

I ran the command sort --help to get the following information

1. ```-n, --numeric-sort          compare according to string numerical value```  

1. ```-r, --reverse               reverse the result of comparisons```  

1. There is but a single dash before single character flags




