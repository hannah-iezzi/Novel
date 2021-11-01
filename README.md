# Novel
Colab code for Novel 

# read Frankenstein file
with open("/content/frankenstein.txt", errors="surrogateescape") as f:
  text = f.read()

novel = text.replace("Frankenstein","Mr. Fluffy")
novel = text.replace("monster","fairy")

with open("/content/frankenstein.txt","w",errors="surrogateescape") as f:
  f.write(novel)
