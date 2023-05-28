# assert_greater_than() works [plain]

    Code
      assert_greater_than(c(2, 3, 1), 3)
    Error <rlang_error>
      'c(2, 3, 1)' is not a number! (length is 3, not 1)

---

    Code
      assert_greater_than(c(2, 3, 4), 2)
    Error <rlang_error>
      'c(2, 3, 4)' is not a number! (length is 3, not 1)

---

    Code
      assert_greater_than("abc", 2)
    Error <rlang_error>
      '"abc"' is not a number! (class is character, not numeric)

---

    Code
      assert_greater_than(list(1, 2, 3), 2)
    Error <rlang_error>
      'list(1, 2, 3)' is not a number! (class is list, not numeric)

---

    Code
      assert_greater_than(c(3, 4, 5), 2)
    Error <rlang_error>
      'c(3, 4, 5)' is not a number! (length is 3, not 1)

---

    Code
      assert_greater_than(factor(4), 2)
    Error <rlang_error>
      'factor(4)' is not a number! (class is factor, not numeric)

---

    Code
      assert_greater_than(TRUE, 2)
    Error <rlang_error>
      'TRUE' is not a number! (class is logical, not numeric)

---

    Code
      assert_greater_than(NULL, 2)
    Error <rlang_error>
      'NULL' is not a number! (class is NULL, not numeric)

# assert_all_greater_than() works [plain]

    Code
      assert_all_greater_than(c(2, 3, 1), 3)
    Error <rlang_error>
      c(2, 3, 1) must all be greater than `3`.

---

    Code
      assert_all_greater_than(c(2, 3, 4), 2)
    Error <rlang_error>
      c(2, 3, 4) must all be greater than `2`.

---

    Code
      assert_all_greater_than(2, 2)
    Error <rlang_error>
      2 must be greater than `2`.

---

    Code
      assert_all_greater_than("abc", 2)
    Error <rlang_error>
      '"abc"' must be numeric, not a character

---

    Code
      assert_all_greater_than(list(1, 2, 3), 2)
    Error <rlang_error>
      'list(1, 2, 3)' must be numeric, not a list

---

    Code
      assert_all_greater_than(c(1, 2, 3), 2)
    Error <rlang_error>
      c(1, 2, 3) must all be greater than `2`.

---

    Code
      assert_all_greater_than(factor(c(1, 2, 3)), 2)
    Error <rlang_error>
      'factor(c(1, 2, 3))' must be numeric, not a factor

---

    Code
      assert_all_greater_than(TRUE, 2)
    Error <rlang_error>
      'TRUE' must be numeric, not a logical

---

    Code
      assert_all_greater_than(NULL, 2)
    Error <rlang_error>
      'NULL' must be numeric, not a NULL

# assert_all_greater_than_or_equal_to() works [plain]

    Code
      assert_all_greater_than_or_equal_to(c(2, 3, 1), 3)
    Error <rlang_error>
      c(2, 3, 1) must all be greater than or equal to `3`.

---

    Code
      assert_all_greater_than_or_equal_to("abc", 2)
    Error <rlang_error>
      '"abc"' must be numeric, not a character

---

    Code
      assert_all_greater_than_or_equal_to(list(1, 2, 3), 2)
    Error <rlang_error>
      'list(1, 2, 3)' must be numeric, not a list

---

    Code
      assert_all_greater_than_or_equal_to(c(1, 2, 3), 2)
    Error <rlang_error>
      c(1, 2, 3) must all be greater than or equal to `2`.

---

    Code
      assert_all_greater_than_or_equal_to(factor(c(1, 2, 3)), 2)
    Error <rlang_error>
      'factor(c(1, 2, 3))' must be numeric, not a factor

---

    Code
      assert_all_greater_than_or_equal_to(TRUE, 2)
    Error <rlang_error>
      'TRUE' must be numeric, not a logical

---

    Code
      assert_all_greater_than_or_equal_to(NULL, 2)
    Error <rlang_error>
      'NULL' must be numeric, not a NULL

---

    Code
      assert_all_greater_than_or_equal_to(NA, 3)
    Error <rlang_error>
      'NA' must be numeric, not a logical

---

    Code
      assert_all_greater_than_or_equal_to(c(4, NA), 3)
    Error <rlang_error>
      'c(4, NA)' must have no missing values! Found 1

# assert_greater_than_or_equal_to() works [plain]

    Code
      assert_greater_than_or_equal_to(2, 3)
    Error <rlang_error>
      2 must be greater than or equal to `3`.

---

    Code
      assert_greater_than_or_equal_to("abc", 2)
    Error <rlang_error>
      '"abc"' is not a number! (class is character, not numeric)

---

    Code
      assert_greater_than_or_equal_to(list(1, 2, 3), 2)
    Error <rlang_error>
      'list(1, 2, 3)' is not a number! (class is list, not numeric)

---

    Code
      assert_greater_than_or_equal_to(c(3, 2, 3), 2)
    Error <rlang_error>
      'c(3, 2, 3)' is not a number! (length is 3, not 1)

---

    Code
      assert_greater_than_or_equal_to(factor(1), 2)
    Error <rlang_error>
      'factor(1)' is not a number! (class is factor, not numeric)

---

    Code
      assert_greater_than_or_equal_to(TRUE, 2)
    Error <rlang_error>
      'TRUE' is not a number! (class is logical, not numeric)

---

    Code
      assert_greater_than(NULL, 2)
    Error <rlang_error>
      'NULL' is not a number! (class is NULL, not numeric)

---

    Code
      assert_greater_than_or_equal_to(NA, 3)
    Error <rlang_error>
      'NA' is not a number! (class is logical, not numeric)

---

    Code
      assert_greater_than_or_equal_to(c(4, NA), 3)
    Error <rlang_error>
      'c(4, NA)' is not a number! (length is 2, not 1)

# assert_identical() works [plain]

    Code
      assert_identical(c(3, 3, 3), 3)
    Error <rlang_error>
      c(3, 3, 3) must be identical to 3

---

    Code
      assert_identical(3, 4)
    Error <rlang_error>
      3 must be identical to 4

---

    Code
      assert_identical(c(1, 2, 3), 3)
    Error <rlang_error>
      c(1, 2, 3) must be identical to 3

---

    Code
      assert_identical(list(1, 2, 3), list(1, 2, 4))
    Error <rlang_error>
      list(1, 2, 3) must be identical to list(1, 2, 4)

---

    Code
      assert_identical(x = length(1:3), y = 3)
    Error <rlang_error>
      length(1:3) must be identical to 3

---

    Code
      assert_identical(c(a = 3), c(b = 3))
    Error <rlang_error>
      c(a = 3) must be identical to c(b = 3)

# assert_equal() works [plain]

    Code
      assert_equal(c(3, 3, 3), 3)
    Error <rlang_error>
      c(3, 3, 3) must be equal to 3

---

    Code
      assert_equal(3, 4)
    Error <rlang_error>
      3 must be equal to 4

---

    Code
      assert_equal(c(1, 2, 3), 3)
    Error <rlang_error>
      c(1, 2, 3) must be equal to 3

---

    Code
      assert_equal(list(1, 2, 3), list(1, 2, 4))
    Error <rlang_error>
      list(1, 2, 3) must be equal to list(1, 2, 4)

---

    Code
      assert_equal(c(a = 3), c(b = 3), check_names = TRUE)
    Error <rlang_error>
      c(a = 3) must be equal to c(b = 3)

