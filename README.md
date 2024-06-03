def find_line(word):
  #word = "Alone"
  data = True
  line_no = 1
  with open("sam_oth.txt", "r") as f:
    while data:
      data = f.readline()
      if (word in data):
        print(line_no)
        return 
      line_no += 1
  return "not found"
  
