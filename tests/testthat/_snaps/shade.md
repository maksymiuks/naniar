# shade errors with NULLs

    Code
      shade(NULL)
    Error <rlang_error>
      Input must not be NULL
      Input is <NULL>

# shade errors with objects of length 0

    Code
      shade(numeric(0))
    Error <rlang_error>
      input to shade must have length > 0

# shade errors with list of length 0

    Code
      shade(list())
    Error <rlang_error>
      input to shade must have length > 0

# shade returns the correct values with list columns

    Code
      shade(list(3, list(1), c(2, 3), list()), broken = 3)
    Error <rlang_error>
      additional levels of missing are not available when shade-ing lists column

