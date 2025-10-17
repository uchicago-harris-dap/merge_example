# merge_example
An in-class example of how to handle merge conflicts

### what has been done so far
| name | branch   | content                                  | parent    | conflict? |
|------|----------|------------------------------------------|-----------|-----------|
| C0   | `main`   | Create `add.py`, which adds x to 3       | none      | no        |
| C1   | `hotfix` | Change `add.py` to add x and y           | C0        | no        |
| C2   | `iss53`  | Change `add.py` to add a list  | C0      | no        |
| C3   | `main`   | Change `add.py` to add x to 4            | C0         | no        |
| C4   | `main`   | Merge `hotfix` into `main`               | C1 \& C3 | yes!      |
| ... | `main`    | improve readme formatting                | C4       | no | 

### what you need to do
| name | branch   | content                                  | parent    | conflict? |
|------|----------|------------------------------------------|-----------|-----------|
| C5   | `main`   | Merge `iss53` into `main`             | C2 \& C4 | yes!      |
