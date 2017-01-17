# Euler's number
Javascript code to get euler's number (accuracy depends on accuracy variable which
obviously just changes how many times it loops through the formula).

    let e = 0;
    let accuracy = 10000;

    function factorial(num) {
      if (num < 0) {
        return -1;
      } else if (num == 0) {
        return 1;
      } else {
        return (num * factorial(num - 1));
      }
    }

    for (let i = 0; i <= accuracy; i++) {
      e += 1/factorial(i);
    }

    console.log(e);
