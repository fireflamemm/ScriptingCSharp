# Walkthrough
1. The most important files for any problem are the AtheneStreamReader.cs and the ProblemRunner.cs file that is in each problem folder. The first reflects all standard input to the standard output (which allows us to have pretty red text for input). The second will actually be running their code. The reason that we need the Runner file is because the Runner file replaces the standard Console StreamReader with the AtheneStreamReader before running the student's code. This means that any time that we input info to the student's program we will get the output we desire (that is that input gets reflected to output with the mangling we desire).
2. Currently, the AtheneStreamReader is a DLL that we can move from place to place. The only issue that I can possibly see with that is if for some reason the DLL doesn't translate nicely from one OS to another. We may need to replace that with a compilation at run time. That or put things in the same namespace. Basically a problem that I will fix when I get back to school in January. With that being said you probably need to recompile this DLL before testing this locally. 

# Instructions for creating new problems (TODO)