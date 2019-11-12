CSE 601: Data Mining and Bioinformatics
Project 1: Dimesionality Reduction and Association Analysis
Part 1: Association Analysis
Submitted By: Karan Manchandia | karanman | 50290755
              Divya Srivastava | divyasri | 50290383
              Varsha Lakshman  | varshala | 50288138

Requirements: Python3.6
	      Jupyter Notebook


Folder Hierarchy: 
> project1
   > PCA
      > PCA_report.pdf
      > Code
   > Association
      > Association_report.pdf
      > Code

How to run the code:
1) Please find the Proj1_Part2.ipynb file inside the Code folder. The Code folder can be found inside the submitted Project folder.
2) Note that in order to run the code you need to place the data file associationruletestdata.txt, inside the same folder in which the Proj1_Part2.ipynb is placed. 
3) Open the Proj1_Part2.ipynb file in the Jupyter Notebook.
4) Run all the cells to see the outputs.
5) Command line inputs-
   >Enter the gene-expression data file name, when prompted.
    Eg- associationruletestdata.txt
   >Enter the minimum support threshold value(in percentage), when prompted.
    Eg- 50
   >Enter the minimum confidence threshold value(in percentage), when prompted.
    Eg- 50
   >Enter the template query in proper format, when prompted.
    Eg- asso_rule.template1("RULE", "ANY", ['G59_Up'])

Required queries:
asso_rule.template1("RULE", "ANY", ['G59_Up'])
asso_rule.template1("RULE", "NONE", ['G59_Up'])
asso_rule.template1("RULE", 1, ['G59_Up', 'G10_Down'])
asso_rule.template1("HEAD", "ANY", ['G59_Up'])
asso_rule.template1("HEAD", "NONE", ['G59_Up'])
asso_rule.template1("HEAD", 1, ['G59_Up', 'G10_Down'])
asso_rule.template1("BODY", "ANY", ['G59_Up'])
asso_rule.template1("BODY", "NONE", ['G59_Up'])
asso_rule.template1("BODY", 1, ['G59_Up', 'G10_Down'])
asso_rule.template2("RULE", 3)
asso_rule.template2("HEAD", 2)
asso_rule.template2("BODY", 1)
asso_rule.template3("1or1", "HEAD", "ANY", ['G10_Down'], "BODY", 1, ['G59_Up'])
asso_rule.template3("1and1", "HEAD", "ANY", ['G10_Down'], "BODY", 1, ['G59_Up'])
asso_rule.template3("1or2", "HEAD", "ANY", ['G10_Down'], "BODY", 2)
asso_rule.template3("1and2", "HEAD", "ANY", ['G10_Down'], "BODY", 2)
asso_rule.template3("2or2", "HEAD", 1, "BODY", 2)
asso_rule.template3("2and2", "HEAD", 1, "BODY", 2)
   