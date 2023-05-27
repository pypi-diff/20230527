# Comparing `tmp/wangticketyes24-0.8-py3-none-any.whl.zip` & `tmp/wangticketyes24-0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 27816 bytes, number of entries: 12
--rw-r--r--  2.0 unx      114 b- defN 23-May-15 13:50 wangticketyes24/__init__.py
--rw-r--r--  2.0 unx    26992 b- defN 23-May-15 13:49 wangticketyes24/selenium_yes24.py
--rw-r--r--  2.0 unx    42099 b- defN 23-Apr-01 09:29 wangticketyes24/yes24.py
+Zip file size: 28236 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      114 b- defN 23-May-27 04:26 wangticketyes24/__init__.py
+-rw-r--r--  2.0 unx    28119 b- defN 23-May-27 04:26 wangticketyes24/selenium_yes24.py
+-rw-r--r--  2.0 unx    43060 b- defN 23-May-27 03:56 wangticketyes24/yes24.py
 -rw-r--r--  2.0 unx       94 b- defN 18-Dec-12 13:54 yes24ticket/__init__.py
 -rw-r--r--  2.0 unx     7490 b- defN 18-Dec-12 14:11 yes24ticket/selenium_yes24.py
 -rw-r--r--  2.0 unx    15460 b- defN 18-Dec-12 14:12 yes24ticket/yes24test.py
--rw-r--r--  2.0 unx       61 b- defN 23-May-15 13:52 wangticketyes24-0.8.dist-info/DESCRIPTION.rst
--rw-r--r--  2.0 unx      690 b- defN 23-May-15 13:52 wangticketyes24-0.8.dist-info/metadata.json
--rw-r--r--  2.0 unx       16 b- defN 23-May-15 13:52 wangticketyes24-0.8.dist-info/top_level.txt
--rw-r--r--  2.0 unx       92 b- defN 23-May-15 13:52 wangticketyes24-0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx      575 b- defN 23-May-15 13:52 wangticketyes24-0.8.dist-info/METADATA
--rw-r--r--  2.0 unx     1034 b- defN 23-May-15 13:52 wangticketyes24-0.8.dist-info/RECORD
-12 files, 94717 bytes uncompressed, 26082 bytes compressed:  72.5%
+-rw-r--r--  2.0 unx       61 b- defN 23-May-27 04:28 wangticketyes24-0.9.dist-info/DESCRIPTION.rst
+-rw-r--r--  2.0 unx      690 b- defN 23-May-27 04:28 wangticketyes24-0.9.dist-info/metadata.json
+-rw-r--r--  2.0 unx       16 b- defN 23-May-27 04:28 wangticketyes24-0.9.dist-info/top_level.txt
+-rw-r--r--  2.0 unx       92 b- defN 23-May-27 04:28 wangticketyes24-0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx      575 b- defN 23-May-27 04:28 wangticketyes24-0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx     1034 b- defN 23-May-27 04:28 wangticketyes24-0.9.dist-info/RECORD
+12 files, 96805 bytes uncompressed, 26502 bytes compressed:  72.6%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: yes24ticket/selenium_yes24.py
 Comment: 
 
 Filename: yes24ticket/yes24test.py
 Comment: 
 
-Filename: wangticketyes24-0.8.dist-info/DESCRIPTION.rst
+Filename: wangticketyes24-0.9.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: wangticketyes24-0.8.dist-info/metadata.json
+Filename: wangticketyes24-0.9.dist-info/metadata.json
 Comment: 
 
-Filename: wangticketyes24-0.8.dist-info/top_level.txt
+Filename: wangticketyes24-0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: wangticketyes24-0.8.dist-info/WHEEL
+Filename: wangticketyes24-0.9.dist-info/WHEEL
 Comment: 
 
-Filename: wangticketyes24-0.8.dist-info/METADATA
+Filename: wangticketyes24-0.9.dist-info/METADATA
 Comment: 
 
-Filename: wangticketyes24-0.8.dist-info/RECORD
+Filename: wangticketyes24-0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wangticketyes24/__init__.py

```diff
@@ -1,5 +1,5 @@
 name = "wangticketyes24"
-__version__ = "0.8"
+__version__ = "0.9"
 
 from .yes24 import Yes24
 from .selenium_yes24 import Selenium_yes24
```

## wangticketyes24/selenium_yes24.py

```diff
@@ -11,14 +11,16 @@
 
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support.ui import Select
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.common.exceptions import TimeoutException
+from selenium.common.exceptions import NoAlertPresentException
+from selenium.common.exceptions import UnexpectedAlertPresentException
 from selenium.common.exceptions import WebDriverException
 
 class Stage(object):
 	START = 0
 	LOGINED = 1
 	PERF_OPENED = 2
 
@@ -432,14 +434,15 @@
 		#티켓 주문처리중 오류가 발생하였습니다.[861]<br>팬클럽 인증 정보가 없습니다. 팬클럽 인증 확인 후 예매하여 주시기 바랍니다.
 		#""
 		ALERT3 = "자동주문방지 문자를 입력해주세요."
 		ALERT4 = "결제를 취소하셨습니다."
 		ALERT5 = "가상계좌 발급중 오류가 발생하였습니다."
 		ALERT6 = "허용 기준을 초과 합니다"
 		ALERT7 = "팬클럽 인증 정보가 없습니다."
+		ALERT8 = "다른 결제 방법을 선택하여 주십시오."
 
 		content = self.driver.find_element_by_xpath("//div[@id='dialogAlert']")
 		contentHTML = content.get_attribute('innerHTML')
 		print("alert is displayed.", contentHTML)
 
 		btn_xpath = "//button[@aria-disabled='false']"
 		e = self.driver.find_element_by_xpath(btn_xpath)
@@ -450,14 +453,16 @@
 			return 1
 		elif ALERT5 in contentHTML:
 			return 3
 		elif ALERT6 in contentHTML:
 			return 4
 		elif ALERT7 in contentHTML:
 			return 5
+		elif ALERT8 in contentHTML:
+			return 6
 		elif ALERT2 in contentHTML or ALERT4 in contentHTML:
 			return 2
 		else:
 			return -1
 
 	def enterOrderPage(self, bookno):
 		## handling popup
@@ -616,14 +621,16 @@
 			totalprice = payprice + giftuse
 			print("totalprice:", totalprice)
 			print("giftuse:", giftuse)
 			if giftuse > 0 and totalprice != giftuse:
 				print("totalprice and giftuse is different! need to change")
 				self.fixGiftAmount(money=totalprice)
 
+			trying_seat = self.driver.execute_script("return document.getElementById('tk_seat').innerText;")
+
 			## checkout button
 			e = self.driver.find_element_by_xpath("//img[@id='imgPayEnd']")
 			self.driver.execute_script("arguments[0].click();", e)
 
 			self.driver.implicitly_wait(1)
 
 			## dialog check
@@ -663,25 +670,46 @@
 						elif ret == 5:
 							msg = "[{}] 팬클럽 미인증 계정".format(self.userid)
 							print(msg)
 							self.notifyTelegram(message=msg)
 							print("Should find new seats after 10seconds")
 							time.sleep(10)
 							return False
+						elif ret == 6:
+							msg = "[{}] 카드결제만 허용?".format(self.userid)
+							print(msg)
+							self.notifyTelegram(message=msg)
+							e = retry_find_element_by_xpath(self.driver, "//input[@idgroup='2']")
+							self.driver.execute_script("arguments[0].click();", e)
+							print("Should click Pay button again.. after select credit card")
+							break
 					elif len(inicis)>0 and inicis[0].is_displayed():
 						print("credit card checkout displayed")
 						self.notifySeatInfo()
 						self.payHyundaiCard()
 						continue
 					elif len(success)>0 and success[0].is_displayed():
 						print("SuccessBoard is ready")
 						return True
 					else:
 						print("nothing displayed...waiting..")
 						continue
+				except UnexpectedAlertPresentException as e:
+					print(traceback.format_exc())
+					# alert text check
+					# 주문이 완료되었습니다.
+					# 이용해 주셔서 감사합니다.
+
+					alert = self.driver.switch_to.alert
+					alertText = alert.text
+					msg = "[{}] alert:{} (seat:{})".format(self.userid, alertText, trying_seat)
+					print(msg)
+					self.notifyTelegram(message=msg)
+					time.sleep(10)
+
 				except WebDriverException as e:
 					print(traceback.format_exc())
 					print("This error temporarily happens in Windows..")
 				time.sleep(1)
 
 			self.driver.implicitly_wait(5)
```

## wangticketyes24/yes24.py

```diff
@@ -158,14 +158,23 @@
 		self.idperf = idperf
 		self.idtime = idtime
 		self.idhall = idhall
 		self.triedSeats = []
 		#self.customerid = None
 		#self.ipmanager = IPManager()
 
+		self.previous_classes = ""
+		self.previous_seatEnd = ""
+
+		self.previous_count = 0
+		self.previous_EtcFee = ""
+
+		self.previous_DeliveryMethod = ""
+		self.previous_idseatclass = ""
+
 	def login(self, loginid, loginpw):
 		self.loginid = loginid
 		self.loginpw = loginpw
 		URL = "http://ticket.yes24.com/Pages/Login/Ajax/AxLoginEnt.aspx"
 		headers = {'User-Agent':'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_11_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.102 Safari/537.36'}
 		payload = {'PLoginID':loginid, 'PPassword':loginpw}
 		r = self.session.post(URL, headers=headers, data=payload)
@@ -527,14 +536,19 @@
 
 	def _lockSeat(self, block, date, idtime, seats):
 		if len(seats) == 0:
 			return False
 
 		self.triedSeats.extend(seats)
 
+		#### TEST CODE [S]
+		print("Lock fake done")
+		return True
+		#### TEST CODE [E]
+
 		mytoken = ",".join([seat.seatid for seat in seats])
 		print(date, idtime, mytoken)
 		[print(seat) for seat in seats]
 		#myptags = "".join([seat.getPTag() for seat in seats])
 		#print(myptags)
 
 		URL = "http://ticket.yes24.com/OSIF/Book.asmx/Lock"
@@ -609,14 +623,20 @@
 fdc_PreCheckPromotion('15962389','34556','84','T','F',1,1,this);
 function fdc_PreCheckPromotionBase(jpIdPromotion, jpIdCode, jpIdAuth, jpIsOverlap, jpIsLimit, jpLimitNo, jpGroupIndex, jpSelObj)
 	"""
 	def _getPromotion(self, seldate, idtime, promo, count):
 		#if promo == "":
 		#	return
 
+		if self.previous_idseatclass == self.idseatclass:
+			print("[Promotion] reusing previous result")
+			return
+
+		self.previous_idseatclass = self.idseatclass
+
 		URL = "http://ticket.yes24.com/Pages/Perf/Sale/Ajax/Perf/PromotionByClass.aspx"
 		headers = {'User-Agent':'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_11_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.102 Safari/537.36'}
 		headers['Content-Type'] = 'application/x-www-form-urlencoded; charset=UTF-8'
 		payload = {'pIdTime': idtime, 'pSelDt': seldate, 'pSeat':self.idseatclass, 'pIdCode': '', 'pHCardAppOpt': 0}
 		print("payload:", payload)
 		r = self.session.post(URL, headers=headers, data=payload)
 		print("[Promotion]", r.status_code, r.reason, r.headers['Date'])
@@ -951,14 +971,18 @@
 	def browser_wait_last_page(self, payment_method=1, deposit=0, giftuse='', captcha_self=False):
 		self.sel.goLastPage()
 		self.sel.prepare_lastpage(payment_method=payment_method, showcaptcha=self.showcaptcha)
 		self.getYesGift(money=deposit, giftuse=giftuse)
 		self.sel.handleCaptcha(captcha_self=captcha_self)
 
 	def _seatEnd(self, idtime, classes):
+		if self.previous_classes == classes:
+			print("[seatEnd] reusing previous result")
+			return self.previous_seatEnd
+
 		URL = "http://ticket.yes24.com/Pages/Perf/Sale/Ajax/Perf/TimeSeatFlashEnd.aspx"
 		#URL = "http://m.ticket.yes24.com/Perf/Sale/Ajax/Perf/AxTimeSeatFlashEnd.aspx"
 		headers = {'User-Agent':'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_11_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.102 Safari/537.36'}
 		payload = {'pIdTime': idtime, 'PCntClass':classes}
 		r = self.session.post(URL, headers=headers, data=payload)
 		print("[seatEnd]", r.status_code, r.reason, r.headers['Date'])
 		#print(r.text)
@@ -968,14 +992,18 @@
 		self.classbyte = soup.find('div')['classbyte']
 		self.price = int(soup.find('select', {"id":"selSeatClass"})['price'] )
 		self.ticketcnt = soup.find('option')['value']
 		self.idseatclassprice = "{}-{}-{},".format(self.classbyte, self.ticketcnt, self.price)
 		self.idseatclass = "{}-{},".format(self.classbyte, self.ticketcnt)
 		#print('IdSeatClassPrice:', self.idseatclassprice)
 		#print('IdSeatClass:', self.idseatclass)
+
+		self.previous_classes = classes
+		self.previous_seatEnd = r.text
+
 		return r.text
 
 	def seatEnd(self, idtime, classes):
 		EXCEPT_COUNT = 0
 		while True:
 			if EXCEPT_COUNT > 100:
 				raise Exception("TOO MUCH EXCEPTION...")
@@ -989,28 +1017,34 @@
 				EXCEPT_COUNT = EXCEPT_COUNT + 1
 				continue
 
 			return result
 
 
 	def _getEtcFee(self, idtime, count):
+		if self.previous_count == count:
+			print("[EtcFee] reusing previous result")
+			return self.previous_EtcFee
+
 		URL = "http://ticket.yes24.com/Pages/Perf/Sale/Ajax/Perf/EtcFee.aspx"
 		#URL = "http://m.ticket.yes24.com/Perf/Sale/Ajax/Perf/AxEtcFee.aspx"
 		headers = {'User-Agent':'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_11_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.102 Safari/537.36'}
 		payload = {'pIdTime': idtime, 'pSeatCnt': count, 'pFreeCountOfCoupon': 0, 'pFreeCountOfGiftTicket': 0}
 		r = self.session.post(URL, headers=headers, data=payload)
 		print("[EtcFee]", r.status_code, r.reason, r.headers['Date'])
 		print(r.text)
 		#<input type=hidden id=EtcFees value='69#2000^' /><input type=hidden id=EtcFeeAmount value='2000' /><input type=hidden id=EtcValidTicketCnt value='2' />
 
 		soup = BeautifulSoup(r.text, "html.parser")
 		self.feetype = soup.find('input', {"id": "EtcFees"})['value']
 		self.feeamount = soup.find('input', {"id": "EtcFeeAmount"})['value']
 		#print(self.feetype)
 		#print(self.feeamount)
+		self.previous_count = count
+		self.previous_EtcFee = r.text
 		return r.text
 
 	def getEtcFee(self, idtime, count):
 		EXCEPT_COUNT = 0
 		while True:
 			if EXCEPT_COUNT > 100:
 				raise Exception("TOO MUCH EXCEPTION...")
@@ -1026,20 +1060,25 @@
 
 			return result
 
 
 	## http://ticket.yes24.com/Pages/Perf/Sale/Scripts/ps_divControls.js?v3=75
 	## fdc_CheckWillCall()
 	def _getDeliveryMethod(self, idtime, date, idperf, idclass):
+		if self.previous_DeliveryMethod != "":
+			print("[DeliveryMethod] reusing previous result")
+			return self.previous_DeliveryMethod
+
 		URL = "http://ticket.yes24.com/Pages/Perf/Sale/Ajax/Perf/DeliveryMethod.aspx"
 		headers = {'User-Agent':'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_11_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.102 Safari/537.36'}
 		payload = {'pIdTime':idtime, 'pBaseDate':date, 'pIdPerf':idperf, 'pIdClass':idclass}
 		r = self.session.post(URL, headers=headers, data=payload)
 		print('[DeliveryMethod]',r.status_code, r.reason, r.headers['Date'])
 		print(r.text)
+		self.previous_DeliveryMethod = r.text
 		return r.text
 
 
 	def getDeliveryMethod(self, idtime, date, idperf, idclass):
 		EXCEPT_COUNT = 0
 		while True:
 			if EXCEPT_COUNT > 100:
```

## Comparing `wangticketyes24-0.8.dist-info/metadata.json` & `wangticketyes24-0.9.dist-info/metadata.json`

 * *Files 0% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'0.9'"}*

```diff
@@ -33,9 +33,9 @@
                 "beautifulsoup4",
                 "requests",
                 "selenium"
             ]
         }
     ],
     "summary": "wangticket for y",
-    "version": "0.8"
+    "version": "0.9"
 }
```

## Comparing `wangticketyes24-0.8.dist-info/METADATA` & `wangticketyes24-0.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: wangticketyes24
-Version: 0.8
+Version: 0.9
 Summary: wangticket for y
 Home-page: https://gitlab.com/wangticket/yes24-ticket
 Author: Wangticket
 Author-email: wangticket77@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `wangticketyes24-0.8.dist-info/RECORD` & `wangticketyes24-0.9.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-wangticketyes24/__init__.py,sha256=2-aIW9w48KQgr5RocuUKNVMGjOTtaiiwHDjXuBsGK2M,114
-wangticketyes24/selenium_yes24.py,sha256=Sq6mxeZGBqHfj1HkErCjeN7Xy50qkmWhSxfHs7tTNMw,26992
-wangticketyes24/yes24.py,sha256=X-RrImHk-hHnO7wE5U28Jx2ow3bwqDbiY3YO0kMmHEY,42099
-wangticketyes24-0.8.dist-info/DESCRIPTION.rst,sha256=iA1-u5zGsM2eQRcqv1-vqBiJevH0U-KhtkZxpjzmfx4,61
-wangticketyes24-0.8.dist-info/METADATA,sha256=nwiuk092CUeJvW-kknIqCI7nktE1w4PkN40KBvZm5QM,575
-wangticketyes24-0.8.dist-info/RECORD,,
-wangticketyes24-0.8.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
-wangticketyes24-0.8.dist-info/metadata.json,sha256=U3tl3vd1LgbYvH30QVzRv4AEY34Wprf5HqgFWo9y15U,690
-wangticketyes24-0.8.dist-info/top_level.txt,sha256=gHGxU_Wfy3Ly7zkKLxm67DoXktNcwN0ImDzlhzNaiW4,16
+wangticketyes24/__init__.py,sha256=-OyKPe-HRsDsrSGNIrn0hDrS78nLI4zS7c05Ehwwrx8,114
+wangticketyes24/selenium_yes24.py,sha256=ehj760D8oJsqTJOGCvyPtF_veEibWULjyZRzA_BPg1U,28119
+wangticketyes24/yes24.py,sha256=vXsSawgcRQ8Vbj8nYPC_g0JKKcz-fMeLfY6Ekg8EKBE,43060
+wangticketyes24-0.9.dist-info/DESCRIPTION.rst,sha256=iA1-u5zGsM2eQRcqv1-vqBiJevH0U-KhtkZxpjzmfx4,61
+wangticketyes24-0.9.dist-info/METADATA,sha256=QKnByf54JZHim-I3OAvFGNCEFObSMfYOx1beQeJMTwM,575
+wangticketyes24-0.9.dist-info/RECORD,,
+wangticketyes24-0.9.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
+wangticketyes24-0.9.dist-info/metadata.json,sha256=HWJfyAi3SJbVjgpc_Bsv84LPZUqwm05bFgjWbbQAm7Y,690
+wangticketyes24-0.9.dist-info/top_level.txt,sha256=gHGxU_Wfy3Ly7zkKLxm67DoXktNcwN0ImDzlhzNaiW4,16
 yes24ticket/__init__.py,sha256=amffzfln3WNiLWWyUul39xXObS4TmQRza8OBgfN24M8,94
 yes24ticket/selenium_yes24.py,sha256=z6ataHl-e3AVhQTZFSYPdn1OfSOklBTizd2mLA57DAM,7490
 yes24ticket/yes24test.py,sha256=6my-oQh4NITv3IkaT_W_v61Z5iPDqNmDU6b3Qx9N5l8,15460
```

