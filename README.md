# Solution for Cafe Class

```python
class Building:
    def __init__(self):
        self.is_open = False

    def open(self):
        self.is_open = True

    def close(self):
        self.is_open = False


class Cafe(Building):
    def __init__(self, name, tables: int, seats_at_table: int):
        super().__init__()
        self.name = name
        self.tables = tables
        self.seats_at_table = seats_at_table

    @property
    def clients_capacity(self):
        return self.tables * self.seats_at_table

```
