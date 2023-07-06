# HandleExceptionServlet
1. Khi click vào Eror Handle, Servet đích sẽ ném ra một ngoại lệ Error và web container sẽ tìm kiếm các xử lý ngoại lệ trong web.xml 
  -> Ngoại lệ sẽ được xử lý bằng cách chuyển hướng tới /handle-exception-servlet.
2. Khi click vào Error with status code thì Servlet đích sẽ ném ra một ngoại lệ và web container sẽ tìm kiếm các xử lý ngoại lệ trong web.xml 
  -> Lỗi được trả về trang lỗi 500 và ngoại lệ được xử lý bằng cách chuyển hướng tới trang 500.jsp.
3. Khi click vào Error type thì Servlet đích sẽ ném ra một ngoại lệ thuộc lớp java.lang.RuntimeException và web container sẽ tìm kiếm các xử lý ngoại lệ trong web.xml
  -> Ngoại lệ sẽ được xử lý bằng cách chuyển hướng tới errorType.jsp
4. Khi truy cập vào 1 URL không tồn tại(404) thì ngoại lệ sẽ được tìm kiếm và xử lý bằng cách chuyển hướng tới trang errorCode.jsp
   
