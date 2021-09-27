# pro
atm
 <title>简易ATM</title>
    <script>
        //1.里面现存有100块钱
        //2.如果存钱，就用输入钱数加上原有存在钱数，之后弹出显示余额提示框
        //3.如果取钱，就减去取的钱数，之后弹出显示余额提示框
        //4.如果显示余额，就输出余额
        //4.如果退出，弹出退出信息提示框
        var saveMoneySum = 0;//最开始总存钱的金额为0
        var drawMoneySum = 0;//最开始总取钱的金额为0
        var yourMoney = 100;//最开始卡里就有的100块
        //通过for和计数器为2达到循环效果
        var num = prompt('输入您的操作：\n1.存钱\n2.取钱\n3.显示余额\n4.退出');//if else if
        //存钱
        if(num = 1){ 
            var saveMoney = prompt('请输入存储金额：');
            saveMoneySum = saveMoneySum + saveMoney;//存钱的总和=存储的金额+本来的钱数
            alert('您的当前余额为：'+ (saveMoneySum - drawMoneySum + 100) + '元');
        }
        //取钱
        else if (num = 2){
            var drawMoney = prompt('请输入取出金额：');
            if (drawMoney <= saveMoneySum - drawMoneySum){
                drawMoneySum = drawMoneySum + drawMoney;
                alert('您的余额为：' + (saveMoneySum - saveMoney + 100) + '元');
            } else {
                alert('账户余额不足');
            }
        //显示余额
         else if (num = 3){
            alert('您的当前余额为：' + (saveMoneySum - saveMoney + 100) + '元');
            }
        //退出
        else if (num = 4){
            continue;
        }
        else{
            alert('系统未识别操作！请重新输入！');
        }

        }while(num !=4);

    </script>
