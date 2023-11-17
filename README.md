class IterableObject:
    def __init__(self, limit):
        self.limit = limit

    def __iter__(self):
        return (x for x in range(self.limit))

iterable = IterableObject(14)

for value in iterable:
    print(value)
