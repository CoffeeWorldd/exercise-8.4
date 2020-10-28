fname = input("Enter file name: ")
fh = open(fname)
lst = list()
for line in fh:
    line= line.rstrip()
    word = line.split()
    for entry in line.split():
        if not entry in lst: 
            lst.append(entry)
lst.sort()
print(lst)
