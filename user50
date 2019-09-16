
Action()
{
	web_url("WebTours", 
		"URL=http://127.0.0.1:1080/WebTours", 
		"TargetFrame=", 
		"Resource=0", 
		"RecContentType=text/html", 
		"Referer=", 
		"Snapshot=t7.inf", 
		"Mode=HTML", 
		LAST);

	lr_think_time(19);

	web_url("sign up now", 
		"URL=http://127.0.0.1:1080/cgi-bin/login.pl?{parUserName}name=&password=&getInfo=true", 
		"TargetFrame=body", 
		"Resource=0", 
		"RecContentType=text/html", 
		"Referer=http://127.0.0.1:1080/WebTours/home.html", 
		"Snapshot=t8.inf", 
		"Mode=HTML", 
		LAST);

	lr_think_time(166);

	lr_start_transaction("1_transaction");

	web_submit_data("login.pl",
		"Action=http://127.0.0.1:1080/cgi-bin/login.pl",
		"Method=POST",
		"TargetFrame=",
		"RecContentType=text/html",
		"Referer=http://127.0.0.1:1080/cgi-bin/login.pl?username=&password=&getInfo=true",
		"Snapshot=t9.inf",
		"Mode=HTML",
		ITEMDATA,
		"Name=username", "Value={NewParam}", ENDITEM,
		"Name=password", "Value={NewParam_1}", ENDITEM,
		"Name=passwordConfirm", "Value={NewParam_1}", ENDITEM,
		"Name=firstName", "Value=name1", ENDITEM,
		"Name=lastName", "Value=name2", ENDITEM,
		"Name=address1", "Value=prost69", ENDITEM,
		"Name=address2", "Value=vrn/leo/398008", ENDITEM,
		"Name=register.x", "Value=41", ENDITEM,
		"Name=register.y", "Value=8", ENDITEM,
		LAST);

	lr_end_transaction("1_transaction",LR_AUTO);

	lr_think_time(19);

	web_url("button_next.gif", 
		"URL=http://127.0.0.1:1080/cgi-bin/welcome.pl?page=menus", 
		"TargetFrame=body", 
		"Resource=0", 
		"RecContentType=text/html", 
		"Referer=http://127.0.0.1:1080/cgi-bin/login.pl", 
		"Snapshot=t10.inf", 
		"Mode=HTML", 
		LAST);
	lr_think_time(22);

	web_url("welcome.pl", 
		"URL=http://127.0.0.1:1080/cgi-bin/welcome.pl?signOff=1", 
		"TargetFrame=", 
		"Resource=0", 
		"RecContentType=text/html", 
		"Referer=http://127.0.0.1:1080/cgi-bin/nav.pl?page=menu&in=home", 
		"Snapshot=t11.inf", 
		"Mode=HTML", 
		LAST);

	return 0;
}
