// 函数节流 
function (fun, delay) {
  let now, last;
  last = new Date().getTime()
  return function () {
    now = new Date().getTime()
    if (now - last > delay) {
      fun();
      last = now;
    }
  }
}
