combs = []
for x in [1,2,3]:
  for y in [3,1,4]:
    if x != y:
      combs.append((x, y))
      
combs

from collections import deque
queue = deque(["Eric", "Jhon", "Michael"])
queue.append("Terry")
queue.append("Graham")
queue.popleft()
queue.popleft()
queue
