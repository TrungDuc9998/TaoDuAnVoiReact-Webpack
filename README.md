<h1 >[Phần 1]&nbsp;Tạo dự án ReactJS với Webpack và Babel</h1>
Link:https://fullstack.edu.vn/blog/phan-1-tao-du-an-reactjs-voi-webpack-va-babel.html
<br>

<div> 
  <h2>NodeJs là gì?Tại sao phải sử dụng node js</h2>
  <p>nodejs:tạo môi trường độc lập để thực thể code javascript trong đó không cần sử dụng các môi trường quen thuộc như trình duyệt</p>
  <p>tạo ra một máy chủ web để chạy trên máy tính của các bạn</p>
  <p>-Không cần sử dụng lặp lại nhiều lần link vì npm sẽ xử lý khi được import</p>
  <p>-Có sẵn luôn cả React,ReactDOM,babel,Webpack</p>
  
  <h2 style="color:red">Tạo dự án với create-react-app</h2>
    <p>Ví dụ bài này chúng ta sẽ tạo ra một dự án với tên là tiktok</p>
    <p>-Đầu tiên chúng ta tạo một folder:843535==>reactjs&&setup</p>
    <p>-Kích chuột phải vào folder reactjs chọn git bash here</p>
    <p>B1:Gõ npx create-react-app sau đó enter sau đó nó sẽ tự tạo ra các thư mục và cấu hình cho dự án,sau khi cài xong thì nó có cái log là success</p>
    <p>npx:là một thư viện giúp chúng ta thực thi các thư viện khác mà không nhất thiết phải cài nó</p>
    <p>B2:di chuyển vào thư mục tiktok chúng ta vừa tạo: "cd tiktok/" nhấn enter</p>
    <p>B3:gõ npm start để chạy dự án</p>
    
    <h2>NPM, NPX và YARN là gì?</h2>
    <p>-NPM:có 2 cách cài</p>
    <p>-Project scope:cài thư viện vào một dự án cụ thể,phụ thuộc vào thư viện
      Để cài thư viện  :npm react react-dom==>dependences
      -cài vào dev denpndences:npm i -D react react-dom
      -xoá thư viện khỏi dự án:npm uninstall react react-dom
      ghi chú:nó đi dowload các thư viện trên npm lưu vào thư mục node_modules sau đó nó list cái dự án vào dependences hoặc devdependences,khi xoá thì làm 
      ngược lại
      -global scope:"/usr/local" hoặc ở chỗ Node được cài,không bị phụ thuộc vào thư viện nào
      -npm i --global create-react-app
      -npm uninstall -g create-react-app
    </p>
   
    <p>-npm:quản lý thư viện được viết bằng javascript</p>
    <p>-Cung cấp website để quản lý thư viện (npm)</p>
    <p>-là một kho lưu trữ</p>
    <p>-là một command-line-interface để tương tác nới npm qua terminal</p>
    <p>có file package-lock.json</p>
    <p>-cài nhiều thư viện cùng một lúc thì cài tuần tự</p>
    <p>-cơ chể cake không tốt như yarn</p>
      
    <p>***yarn:trình quản lý gói khác,cải thiện vấn đề mà npm gặp phải/p>
    <p>có file yarn.json</p>
    <p>Cài nhiều thư viện cùng một lúc thì cài song song có thể nhanh hơn npm</p>
    <p>-Tốn dung lượng lưu trữ khi cake</p>
    
    
    <h2 style="color:red">Hooks là gì</h2>
    <p>-là method ,hàm được viết sẵn ,được cung cấp bởi reactjs,mỗi hàm có mỗi tính năng là các trường hơpk
      cụ thể để chúng ta có thể sử dụng</p>
    <h4>1.useState:trạng thái của dữ liệu,khi dữ liệu thay đổi thì giao
    diện được câoj nhật</h4>
  
  <h2  style="color:red">Two-way binding trong React?</h2>
  
  <h1 style="text-align:center">Giới thiệu react</h1>
<hr/>
<h2 style="color:red">Biến React ES6</h2>
  <h1>Var</h1>
  <p>-Nếu sử dụng biến bên ngoài một chức năng,nó thuộc phạm vi toàn cục</>
    <p>-Nếu sử dụng biến bên trong một chức năng,nó thuộc về chức năng đó</p>
    <p>Nếu sử dụng bên trong một khối,tức là vòng for,thì biến vẫn có sẵn bên ngoài khối đó</p>
    <p>==>var có phạm vi chức năng,không phải phạm vi khối</p>
    <h2>let</p>
    <p>là phiên bản phạm vi khối var và được giới hạn trong khối(hoặc biểu thức) nơi nó được xác định</p>
    <p>-Nếu bạn sử dụng let bên trong một khối,tức là vòng lặp for,thì biến chỉ có sẵn bên trong vòng lặp đó</p>
    <p>==>let có phạm vi khối</p>
    <h2>const :là một biến mà một khi nó được tạo ra,giá trị của nó không bao giờ có thể thay đổi</h2>
    <p>==>const có phạm vi khối</p>
    <p>const:không thể gán lại một giá trị,gián lại một mảng,gán lại một object</p>
    <p>const có thể thay đổi:-các phần tử của mảng trong hằng số,thay đổi thuộc tính đối tượng hàm</p>
<h2 style="color:red">React là gì</h2>
<p>-React đôi khi được gọi là khung js giao diện người dùng,là thư viện js do facebook tạo ta</p>
<p>-React là công cụ để xây dựng các thành phần giao diện người dùng</p>
<h2 style="color:red">React hoạt động như nào</h2>
<p>-React tạo ta một DOM VIRTUAL trong bộ nhớ</p>
<p>-Thay vì phải thao tác trực tiếp với DOM của trình duyệt,React tạo ra một DOM  ảo trong bộ nhớ,
nơi nó thực hiện tất cá các thao tác cần thiết,trước khi thực hiện thay đổi DOM của trình duyệt</p>
<p></p>
<p></p>
<p></p>
<p></p>
<p></p>
<p></p>
<p></p>
<p></p>
<p></p>
<p></p>
<p></p>
<p></p>
<p></p>
<p></p>
<p></p>
<p></p>
<p></p>
<p></p>
<p></p>
<p></p>
  
</div>

