# convert-binary-in-linked-list-to-integer
Code Challenge - Javascript

var getDecimalValue = function(head) {
  let binary = String(head.val);
  
  while (head.next !== null) {
    head = head.next;
    binary += head.val;
  }
  
  return parseInt(binary, 2);
};

Blog with Explanation:
https://medium.com/@yinazee/convert-binary-number-in-a-linked-list-to-integer-1a7f9ea828d7
