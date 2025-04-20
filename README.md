# Operating-System-Lab_Project
## Smart Restaurant Management System
 - `chmod +x filename`
 - `./filename`
 
 ---

- ` bash online compiler link: https://www.onlinegdb.com/online_bash_shell`

 ---



```bash
#!/bin/bash
total_price=0
Choice_item()
{
echo
echo -n "Please choice the item: "
read choice
case $choice in
1) echo "Which quantity of Morogh Pulao?"
echo "1. Half/2. Full"
echo -n "Enter Choice: "
read quantity
        if [ $quantity == 1 ]
        then
        echo -n "How many Morogh Pulao do you want?: "
        read MP_quantity
        price=`expr $MP_quantity \* 110`
        total_price=`expr $total_price + $price`
        echo -n "Would you like to take another item? yes/no: "
        read ai
        if [ $ai == yes ]
        then
        Choice_item
        else
        return 1
        fi
        elif [ $quantity == 2 ]
        then
        echo -n "How many Morogh Pulao do you want?: "
        read MP_quantity
        price=`expr $MP_quantity \* 160`
        total_price=`expr $total_price + $price`
        echo -n "Would you like to take another item? yes/no: "
        read ai
        if [ $ai == yes ]
        then
        Choice_item
        else
        return 1
        fi
        fi;;
2) echo "Which quantity of Mutton Kacchi?"
echo "1. Half/2. Full"
echo -n "Enter Choice: "
read quantity
        if [ $quantity == 1 ]
        then
        echo -n "How many Mutton Kacchi do you want?: "
        read MK_quantity
        price=`expr $MK_quantity \* 120`
        total_price=`expr $total_price + $price`
        echo -n "Would you like to take another item? yes/no: "
        read ai
        if [ $ai == yes ]
        then
        Choice_item
        else
        return 1
        fi
        elif [ $quantity == 2 ]
        then
        echo -n "How many Mutton Kacchi do you want?: "
        read MK_quantity
        price=`expr $MK_quantity \* 180`
        total_price=`expr $total_price + $price`
        echo -n "Would you like to take another item? yes/no: "
        read ai
        if [ $ai == yes ]
        then
        Choice_item
        else
        return 1
        fi
        fi;;
3) echo -n "How many Coffee do you want?: "
        read C_quantity
        price=`expr $C_quantity \* 50`
        total_price=`expr $total_price + $price`
        echo -n "Would you like to take another item? yes/no: "
        read ai
        if [ $ai == yes ]
        then
        Choice_item
        else
        return 1
        fi;;
4) echo -n "How many Orange Juice do you want?: "
        read OJ_quantity
        price=`expr $OJ_quantity \* 60`
        total_price=`expr $total_price + $price`
        echo -n "Would you like to take another item? yes/no: "
        read ai
        if [ $ai == yes ]
        then
        Choice_item
        else
        return 1
        fi;;
5) echo -n "How many Apple Juice do you want?: "
        read AJ_quantity
        price=`expr $AJ_quantity \* 70`
        total_price=`expr $total_price + $price`
        echo -n "Would you like to take another item? yes/no: "
        read ai
        if [ $ai == yes ]
        then
        Choice_item
        else
        return 1
        fi;;
6) echo "Which quantity of Cocacola?"
echo "1. 250ml/2. 600ml/3. 1000ml"
echo -n "Enter Choice: "
read quantity
        if [ $quantity == 1 ]
        then
        echo -n "How many Cocacola do you want?: "
        read Cola_quantity
        price=`expr $Cola_quantity \* 20`
        total_price=`expr $total_price + $price`
        echo -n "Would you like to take another item? yes/no: "
        read ai
        if [ $ai == yes ]
        then
        Choice_item
        else
        return 1
        fi
        elif [ $quantity == 2 ]
        then
        echo -n "How many Cocacola do you want?: "
        read Cola_quantity
        price=`expr $Cola_quantity \* 35`
        total_price=`expr $total_price + $price`
        echo -n "Would you like to take another item? yes/no: "
        read ai
        if [ $ai == yes ]
        then
        Choice_item
        else
        return 1
        fi
        elif [ $quantity == 3 ]
        then
        echo -n "How many Cocacola do you want?: "
        read Cola_quantity
        price=`expr $Cola_quantity \* 60`
        total_price=`expr $total_price + $price`
        echo -n "Would you like to take another item? yes/no: "
        read ai
        if [ $ai == yes ]
        then
        Choice_item
        else
        return 1
        fi
        fi;;
7) echo "Which quantity of Chicken Grill?"
echo "1. Half/2. Full"
echo -n "Enter Choice: "
read quantity
        if [ $quantity == 1 ]
        then
        echo -n "How many Chicken Grill do you want?: "
        read CG_quantity
        price=`expr $CG_quantity \* 160`
        total_price=`expr $total_price + $price`
        echo -n "Would you like to take another item? yes/no: "
        read ai
        if [ $ai == yes ]
        then
        Choice_item
        else
        return 1
        fi
        elif [ $quantity == 2 ]
        then
        echo -n "How many Chicken Grill do you want?: "
        read CG_quantity
        price=`expr $CG_quantity \* 320`
        total_price=`expr $total_price + $price`
        echo -n "Would you like to take another item? yes/no: "
        read ai
        if [ $ai == yes ]
        then
        Choice_item
        else
        return 1
        fi
        fi;;
8) echo -n "How many Naan Roti do you want?: "
        read NR_quantity
        price=`expr $NR_quantity \* 25`
        total_price=`expr $total_price + $price`
        echo -n "Would you like to take another item? yes/no: "
        read ai
        if [ $ai == yes ]
        then
        Choice_item
        else
        return 1
        fi;;
9) echo "Which quantity of Chicken Chaap?"
echo "1. Half/2. Full"
echo -n "Enter Choice: "
read quantity
        if [ $quantity == 1 ]
        then
        echo -n "How many Chicken Chaap do you want?: "
        read CC_quantity
        price=`expr $CC_quantity \* 70`
        total_price=`expr $total_price + $price`
        echo -n "Would you like to take another item? yes/no: "
        read ai
        if [ $ai == yes ]
        then
        Choice_item
        else
        return 1
        fi
        elif [ $quantity == 2 ]
        then
        echo -n "How many Chicken Chaap do you want?: "
        read CC_quantity
        price=`expr $CC_quantity \* 120`
        total_price=`expr $total_price + $price`
        echo -n "Would you like to take another item? yes/no: "
        read ai
        if [ $ai == yes ]
        then
        Choice_item
        else
        return 1
        fi
        fi;;
10) echo -n "How many bowls of vegetables do you want?: "
        read V_quantity
        price=`expr $V_quantity \* 25`
        total_price=`expr $total_price + $price`
        echo -n "Would you like to take another item? yes/no: "
        read ai
        if [ $ai == yes ]
        then
        Choice_item
        else
        return 1
        fi
esac
}
echo "-----------------------------------------------------------------"
echo "              Smart Restaurant Management System"
echo "-----------------------------------------------------------------"
echo "===================Welcome to our Restaurant====================="
echo
echo "============================Food Menu============================"
echo
echo "|Item_No.|=======Food Name=======|====Quantity====|====Price====|"
echo "|   1    | Morogh Pulao          | Half/Full      | 110Tk/160Tk |"
echo "|   2    | Mutton Kacchi         | Half/Full      | 120Tk/180Tk |"
echo "|   3    | Coffee                | 200ml          | 50Tk        |"
echo "|   4    | Orange Juice          | 250ml          | 60Tk        |"
echo "|   5    | Apple Juice           | 250ml          | 70Tk        |"
echo "|   6    | Cocacola              | 250/600/1000ml | 20/35/60Tk  |"
echo "|   7    | Chicken Grill         | Half/Full      | 160/320Tk   |"
echo "|   8    | Naan Roti             | 1 Pec          | 25Tk        |"
echo "|   9    | Chicken Chaap         | Half/Full      | 70/120Tk    |"
echo "|   10   | Vegetables            | 1 Bowl         | 25Tk        |"
echo

echo -n "Do you want to order food? yes/no: "
read ch
case $ch in
yes) echo "Thank You!"
echo "| 1. Table No.01/ 2. Table No.02/ 3. Table No.03/ 4. Table No.04|"
echo -n "Please Select Your Table No.: "
read table_choice
Choice_item
echo 
echo "From Table No. $table_choice"
echo "Your Total Bill = $total_price Tk"
echo "Please Pay Your Bill.!"
echo
echo "Our Payment Method is: "
echo "1. Online Payment / 2. Hand Cash Payment"
echo -n "Choice any payment method: "
read payment
case $payment in
1)
  if [ $total_price -le 50000 ]
      then
      echo
      echo "Successfully Paid Your Bill..!"
      echo
      echo "Thank you so much. Please come again.!"
  else 
      echo "Sorry..! You Don't Have Sufficient Balance!"
  fi;;
2) echo -n "Pay Bill: "
read Bill
    if [ $Bill == $total_price ]
    then
    echo
    echo "Paid Your Bill..!"
    echo "You Pay $Bill Tk and Your Total Bill $total_price Tk"
    echo
    echo "Thank you so much. Please come again.!"
    elif [ $Bill -gt $total_price ]
    then
    change=`expr $Bill - $total_price`
    echo
    echo "Paid Your Bill..!"
    echo "You Pay $Bill Tk but Your Total Bill $total_price Tk"
    echo "So, you will get money = $change Tk"
    echo
    echo "Thank you so much. Please come again.!"
    else
    echo
    echo "Sorry..! Your Total Bill $total_price Tk but You Pay $Bill Tk"
      echo -n "Please paid our due bill: "
      read due
      due_bill=`expr $Bill + $due`
        if [ $due_bill == $total_price ]
        then
        echo
        echo "Okay Paid Your Bill..!"
        echo
        echo "Thank you so much. Please come again.!"
        elif [ $due_bill -gt $total_price ]
        then
        change=`expr $due_bill - $total_price`
        echo
        echo "Okay Paid Your Bill..!"
        echo "You Pay $due_bill Tk but Your Total Bill $total_price Tk"
        echo "So, you will get money = $change Tk"
        echo
        echo "Thank you so much. Please come again.!"
        fi
    fi;;
  esac;;
no) echo
echo "Thank you so much.!";;
esac

```

---

### Output
<div style="text-align: center;">
  <img src="https://ibb.co.com/Q3hdpLMm" alt="Image" style="width: 100%;" />
</div>

---

