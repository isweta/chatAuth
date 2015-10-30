<%@page import="java.io.FileInputStream"%>
<%@page import="java.io.File"%>
<%@page import="java.io.InputStreamReader"%>
<%@page import="java.net.URL"%>
<%@page import="java.io.FileReader"%>
<%@page import="java.io.BufferedReader"%>

<%@ page language="java" contentType="text/html; charset=ISO-8859-1"
    pageEncoding="ISO-8859-1"%>
<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
<html>
<head>
</head>
<body  background="back.jpg">


<center><font face="arial" color="blue" size="6" ><i>Configure </i></font></center>

<Form action="ConfigureServlet">
<table><tr>
<td>TriggerId</td>

  <td><input type="text" name="trigID" ></td>
  </tr>

  <tr>
   <td>ResourceVal:</td>  <td><input type="text" name="resVal" >
</td></tr>
<tr><td></td>
<td><input type="submit" value="submit"></td></tr>
</Form>

</body>
</html>