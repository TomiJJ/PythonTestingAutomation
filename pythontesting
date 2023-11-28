import unittest

def add(x, y):
    return x + y

def multiply(x, y):
    return x * y

def power(x, y):
    """Calculate x raised to the power y without using math.pow."""
    result = 1
    for _ in range(int(y)):
        result *= x
    return result

print(add(5,4))       # --> 9
print(multiply(3,4))  # --> 12
print(power(2,8))     # --> 256


class TestCalc(unittest.TestCase):
    def test_add(self):
        self.assertEqual(add(5, 5), 10)
        self.assertEqual(add(-3, 3), 0)
        self.assertEqual(add(-5,-5),-10)
    def test_multiply(self):
        self.assertEqual(multiply(20, 5), 100)
        self.assertEqual(multiply(-2, 1),-2)
        self.assertEqual(multiply(-1,-3), 3)
    def test_power(self):
        self.assertEqual(power(2, 3), 8)
        self.assertEqual(power(1, 4),1)
        self.assertEqual(power(3,1), 3)
if __name__ == '__main__':
   unittest.main()
