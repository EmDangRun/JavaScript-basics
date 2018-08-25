# JavaScript-basics
1. Sự khác nhau giữa var, let, const 
  - var: 
        + Khi báo biến, bạn có thể thay đổi giá trị cho biến ở bất kì ' trong hay ngoài scope ' ( scope nghĩa là {} )
           vd: var a = 0 
               {
                 a = 4;
               }
               console.log(a);
           kq: a = 4
         + Hỗ trợ hoisting
           vd: a = 4;
               var a;
               console.log(a);
           kq: a = 4  
         + Có thể tạo nhiều biến có tên giống nhau trong cùng 1 scope
           vd: var a = 0;
               var a = 3;
  - let: + Giá trị của biến được quy định theo scope
           vd: let a = 0;
               {
                let a = 4;
               }
               console.log(a);
           kq : a = 0;
         + Khỗng hỗ trợ hoisting
         + Không thể tạo biến có tên giống nhau
         
  - const: + Giá trị của biến giữ nguyên
           + Không hỗ trợ hoisting
           + Không thể tạo biến giống nhau
