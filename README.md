# -study---function-to-change-local-variable-

## 전역변수 없이 함수 내에서 변수값 변경/호출



```javascript
const STATE = updateState();
function updateState() {
    // const state = '<c:out value="${param.state}" />';
    const state = 1;

    function changeState(updatedState) {
        return updatedState ?? state;
    }
    return changeState;
}


console.log(STATE());

//state값 변경
console.log(STATE(0));
console.log(STATE(2));
```
