<meta name="google-site-verification" content="M-EL9z_9rLH5lnUgtP_yUfDNjvodsiUC_8Z86W37iII" />

# StupidAutronic
Trigger calculator for Autronic SM4 antique obsolete ECU's that have unintelligible documentation and use impossible input parameters and vocabulary

For anyone unlucky (or stupid) enough to have to setup an old Autronic SM4 ECU for a missing tooth trigger pattern on some vehicle that doesn't have a pre-configured template, there traditionally were very few options that will get you a working solution. Even though the software presents you with what looks to be lovely "60-2" and "36-1" type trigger options, you still must face the misery of the DIVIDER OFFSET and the CYLINDER INPUT LEAD fields...  In order of "least to most painful" your options were... 

1. Shoot yourself in the face
2. Have someone else shoot you in the face
3. Leap in front of a speeding mass-transit vehicle
3. Hunt down some rare internetzpersonz who have been around long enough to have known and understoond Autronic triggers, and yet still are not so aged as to have forgotten everything about it, and, were not driven insane in the process... Then beg them to understand your situation and tell you what to put into the impossibly arcane user interface. 
4. Attempt to actually read THE DICK's documentation in the software and manual explaining what the vocabulary in the software means, and how to get from easy to understand real-world parameters like "how many teeth is it from TDC1 to the gap?" and "where does my sync trigger occur?" to the hideous and moronic "CYLINDER INPUT LEAD" and "DIVIDER OFFSET" in the hideously stupid user interface (Funfact "I/P is for "IN PUTS" and "O/P" is for "OUT PUTS"!  Who knew Australians spelled INPUT and OUTPUT as 2 words!?)

Anyway.  

Here's a spreadsheet. 

It takes basic shit that normal people can look at their engine and measure and understand, calculates the BLOWTRONIC numbers you need, then, as an added super fun bonus, makes a little map so you actually understand what the numbers mean and what THE DICK is getting at with his weirdo vocabulazry. 

It should work for either the 36-1 or 60-2 or M02 / M12 type choices in Autronic. It def won't work with tooth counts vs cylinder vs stroke configs that result in fractional outputs. If you get shit like "4.5 teeth" obviously that's not gonna work, since DIVIDER OFFSET is a whole tooth count. You'll want to override up/down a tooth.  I have no idea if all the permutations work, it might very well miscalculate if you have a 2-stroke 3-cylinder Saab Sonnett with a 78-4 tooth count trigger and the sync occurring at 341 degrees.  But.... that brings us to... 

Disclaimer time: It might be buggy. It might assplode your enginemotors. If it doesn't work or you have other problems, I barely know anything about Autronic except that I hate the vocabulary and documentation with the red hot fire of 1000 suns, so, don't ask me for help. 

But I do hope it helps somebody. 
