# Comparing `tmp/betfair_parser-0.2.2.tar.gz` & `tmp/betfair_parser-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betfair_parser-0.2.2.tar", max compression
+gzip compressed data, was "betfair_parser-0.2.3.tar", max compression
```

## Comparing `betfair_parser-0.2.2.tar` & `betfair_parser-0.2.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0        0 2023-05-24 06:39:57.992048 betfair_parser-0.2.2/betfair_parser/__init__.py
--rw-r--r--   0        0        0      919 2023-02-24 04:45:44.811742 betfair_parser-0.2.2/betfair_parser/core.py
--rw-r--r--   0        0        0        0 2023-02-17 06:17:12.706435 betfair_parser-0.2.2/betfair_parser/spec/__init__.py
--rw-r--r--   0        0        0       85 2023-05-22 03:56:48.978534 betfair_parser-0.2.2/betfair_parser/spec/accounts/__init__.py
--rw-r--r--   0        0        0     2929 2023-05-22 03:56:48.978762 betfair_parser-0.2.2/betfair_parser/spec/accounts/enums.py
--rw-r--r--   0        0        0     3166 2023-05-22 03:56:48.978966 betfair_parser-0.2.2/betfair_parser/spec/accounts/operations.py
--rw-r--r--   0        0        0    10865 2023-05-22 03:56:48.979202 betfair_parser-0.2.2/betfair_parser/spec/accounts/type_definitions.py
--rw-r--r--   0        0        0       84 2023-05-22 03:56:48.979357 betfair_parser-0.2.2/betfair_parser/spec/betting/__init__.py
--rw-r--r--   0        0        0    20833 2023-05-22 03:56:48.979639 betfair_parser-0.2.2/betfair_parser/spec/betting/enums.py
--rw-r--r--   0        0        0     9485 2023-05-22 03:56:48.979862 betfair_parser-0.2.2/betfair_parser/spec/betting/listings.py
--rw-r--r--   0        0        0      134 2023-05-22 03:56:48.979989 betfair_parser-0.2.2/betfair_parser/spec/betting/operations.py
--rw-r--r--   0        0        0     8706 2023-05-22 03:56:48.980198 betfair_parser-0.2.2/betfair_parser/spec/betting/orders.py
--rw-r--r--   0        0        0    29194 2023-05-23 10:44:45.059729 betfair_parser-0.2.2/betfair_parser/spec/betting/type_definitions.py
--rw-r--r--   0        0        0     5596 2023-05-23 10:44:45.060370 betfair_parser-0.2.2/betfair_parser/spec/common.py
--rw-r--r--   0        0        0      717 2023-05-20 01:56:57.285784 betfair_parser-0.2.2/betfair_parser/spec/constants.py
--rw-r--r--   0        0        0     7970 2023-05-22 03:56:48.980964 betfair_parser-0.2.2/betfair_parser/spec/error.py
--rw-r--r--   0        0        0     1768 2023-05-20 01:56:57.286037 betfair_parser-0.2.2/betfair_parser/spec/heartbeat.py
--rw-r--r--   0        0        0     4300 2023-05-24 06:32:22.808750 betfair_parser-0.2.2/betfair_parser/spec/navigation.py
--rw-r--r--   0        0        0     2966 2023-05-22 03:56:48.981177 betfair_parser-0.2.2/betfair_parser/spec/race_status.py
--rw-r--r--   0        0        0      324 2023-02-17 06:17:12.708820 betfair_parser-0.2.2/betfair_parser/spec/streaming/__init__.py
--rw-r--r--   0        0        0     6274 2023-05-20 01:56:57.286455 betfair_parser-0.2.2/betfair_parser/spec/streaming/mcm.py
--rw-r--r--   0        0        0     2241 2023-05-20 01:56:57.286612 betfair_parser-0.2.2/betfair_parser/spec/streaming/ocm.py
--rw-r--r--   0        0        0     2416 2023-05-20 01:56:57.286756 betfair_parser-0.2.2/betfair_parser/spec/streaming/status.py
--rw-r--r--   0        0        0     2148 2023-05-20 01:56:57.286841 betfair_parser-0.2.2/betfair_parser/strenums.py
--rw-r--r--   0        0        0      645 2023-05-24 06:40:33.480563 betfair_parser-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 betfair_parser-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-24 06:39:57.992048 betfair_parser-0.2.3/betfair_parser/__init__.py
+-rw-r--r--   0        0        0      919 2023-02-24 04:45:44.811742 betfair_parser-0.2.3/betfair_parser/core.py
+-rw-r--r--   0        0        0        0 2023-02-17 06:17:12.706435 betfair_parser-0.2.3/betfair_parser/spec/__init__.py
+-rw-r--r--   0        0        0       85 2023-05-22 03:56:48.978534 betfair_parser-0.2.3/betfair_parser/spec/accounts/__init__.py
+-rw-r--r--   0        0        0     2929 2023-05-22 03:56:48.978762 betfair_parser-0.2.3/betfair_parser/spec/accounts/enums.py
+-rw-r--r--   0        0        0     3127 2023-05-27 00:39:32.172273 betfair_parser-0.2.3/betfair_parser/spec/accounts/operations.py
+-rw-r--r--   0        0        0    11161 2023-05-27 00:39:32.172518 betfair_parser-0.2.3/betfair_parser/spec/accounts/type_definitions.py
+-rw-r--r--   0        0        0       84 2023-05-22 03:56:48.979357 betfair_parser-0.2.3/betfair_parser/spec/betting/__init__.py
+-rw-r--r--   0        0        0    20833 2023-05-22 03:56:48.979639 betfair_parser-0.2.3/betfair_parser/spec/betting/enums.py
+-rw-r--r--   0        0        0     9556 2023-05-27 00:39:32.172747 betfair_parser-0.2.3/betfair_parser/spec/betting/listings.py
+-rw-r--r--   0        0        0      134 2023-05-22 03:56:48.979989 betfair_parser-0.2.3/betfair_parser/spec/betting/operations.py
+-rw-r--r--   0        0        0     8762 2023-05-27 00:39:32.172968 betfair_parser-0.2.3/betfair_parser/spec/betting/orders.py
+-rw-r--r--   0        0        0    29242 2023-05-27 00:39:32.173280 betfair_parser-0.2.3/betfair_parser/spec/betting/type_definitions.py
+-rw-r--r--   0        0        0     5811 2023-05-27 00:39:32.173519 betfair_parser-0.2.3/betfair_parser/spec/common.py
+-rw-r--r--   0        0        0      923 2023-05-27 00:39:32.173730 betfair_parser-0.2.3/betfair_parser/spec/constants.py
+-rw-r--r--   0        0        0     7970 2023-05-22 03:56:48.980964 betfair_parser-0.2.3/betfair_parser/spec/error.py
+-rw-r--r--   0        0        0     1775 2023-05-27 00:39:32.173931 betfair_parser-0.2.3/betfair_parser/spec/heartbeat.py
+-rw-r--r--   0        0        0     4181 2023-05-27 00:39:32.174126 betfair_parser-0.2.3/betfair_parser/spec/navigation.py
+-rw-r--r--   0        0        0     2975 2023-05-27 00:39:32.174337 betfair_parser-0.2.3/betfair_parser/spec/race_status.py
+-rw-r--r--   0        0        0      324 2023-02-17 06:17:12.708820 betfair_parser-0.2.3/betfair_parser/spec/streaming/__init__.py
+-rw-r--r--   0        0        0     6233 2023-05-27 00:39:32.174546 betfair_parser-0.2.3/betfair_parser/spec/streaming/mcm.py
+-rw-r--r--   0        0        0     2247 2023-05-27 00:39:32.174723 betfair_parser-0.2.3/betfair_parser/spec/streaming/ocm.py
+-rw-r--r--   0        0        0     2422 2023-05-27 00:39:32.174911 betfair_parser-0.2.3/betfair_parser/spec/streaming/status.py
+-rw-r--r--   0        0        0     2148 2023-05-20 01:56:57.286841 betfair_parser-0.2.3/betfair_parser/strenums.py
+-rw-r--r--   0        0        0      645 2023-05-27 07:33:29.403575 betfair_parser-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 betfair_parser-0.2.3/PKG-INFO
```

### Comparing `betfair_parser-0.2.2/betfair_parser/core.py` & `betfair_parser-0.2.3/betfair_parser/core.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.2/betfair_parser/spec/accounts/enums.py` & `betfair_parser-0.2.3/betfair_parser/spec/accounts/enums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.2/betfair_parser/spec/accounts/operations.py` & `betfair_parser-0.2.3/betfair_parser/spec/accounts/operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,62 +10,61 @@
 from betfair_parser.spec.common import APIException, BaseMessage, Request, Response, TimeRange
 from betfair_parser.spec.error import AccountAPIExceptionCode
 
 
 AccountAPIException = APIException[AccountAPIExceptionCode]
 
 
-class getAccountFundsParams(BaseMessage, frozen=True):
+class _GetAccountFundsParams(BaseMessage, frozen=True):
     wallet: Optional[Wallet] = None  # Name of the wallet in question. Global wallet is returned by default
 
 
-class getAccountFunds(Request, kw_only=True, frozen=True):
+class GetAccountFunds(Request, kw_only=True, frozen=True):
     """Returns the available to bet amount, exposure and commission information."""
 
     method = "AccountAPING/v1.0/getAccountFunds"
-    params: getAccountFundsParams
+    params: _GetAccountFundsParams
     return_type = Response[AccountFundsResponse]
     throws = AccountAPIException
 
 
-class getAccountDetails(Request, kw_only=True, frozen=True):
+class GetAccountDetails(Request, kw_only=True, frozen=True):
     """Returns the details relating your account, including your discount rate and Betfair point balance."""
 
     method = "AccountAPING/v1.0/getAccountDetails"
     return_type = Response[AccountDetailsResponse]
     throws = AccountAPIException
 
 
-class getAccountStatementParams(BaseMessage, frozen=True):
+class _GetAccountStatementParams(BaseMessage, frozen=True):
     locale: Optional[str] = None  # The language to be used where applicable. Defaults to account settings
-    fromRecord: Optional[int] = None  # Specifies the first record that will be returned, defaults to 0
-    recordCount: Optional[int] = None  # Specifies the maximum number of records to be returned. Maximum 100
-    return_type = Response[AccountDetailsResponse]
+    from_record: Optional[int] = None  # Specifies the first record that will be returned, defaults to 0
+    record_count: Optional[int] = None  # Specifies the maximum number of records to be returned. Maximum 100
 
     # Return items with an itemDate within this date range. Both from and to date times are inclusive.
     # If from is not specified then the oldest available items will be in range. If to is not specified
     # then the latest items will be in range. nb. This itemDataRange is currently only applied when
     # includeItem is set to ALL or not specified, else items are NOT bound by itemDate.
     # Please note:  You can only retrieve account statement items for the last 90 days.
-    itemDateRange: Optional[TimeRange] = None
-    includeItem: Optional[IncludeItem] = None  # Which items to include, if not specified then defaults to ALL.
+    item_date_range: Optional[TimeRange] = None
+    include_item: Optional[IncludeItem] = None  # Which items to include, if not specified then defaults to ALL.
     wallet: Optional[Wallet] = None  # Which wallet to return statementItems for. Defaults to UK
 
 
-class getAccountStatement(Request, kw_only=True, frozen=True):
+class GetAccountStatement(Request, kw_only=True, frozen=True):
     method = "AccountAPING/v1.0/getAccountStatement"
-    params: getAccountStatementParams
+    params: _GetAccountStatementParams
     return_type = Response[AccountStatementReport]
     throws = AccountAPIException
 
 
-class listCurrencyRatesParams(BaseMessage, frozen=True):
-    fromCurrency: Optional[str] = None  # The currency from which the rates are computed. Only GBP for now.
+class _ListCurrencyRatesParams(BaseMessage, frozen=True):
+    from_currency: Optional[str] = None  # The currency from which the rates are computed. Only GBP for now.
 
 
-class listCurrencyRates(Request, kw_only=True, frozen=True):
+class ListCurrencyRates(Request, kw_only=True, frozen=True):
     """Returns a list of currency rates based on given currency. Updates only once per hour."""
 
     method = "AccountAPING/v1.0/listCurrencyRates"
-    params: listCurrencyRatesParams
+    params: _ListCurrencyRatesParams
     return_type = Response[list[CurrencyRate]]
     throws = AccountAPIException
```

### Comparing `betfair_parser-0.2.2/betfair_parser/spec/accounts/type_definitions.py` & `betfair_parser-0.2.3/betfair_parser/spec/accounts/type_definitions.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,226 +10,230 @@
 )
 from betfair_parser.spec.common import BaseMessage, Date
 
 
 class ApplicationSubscription(BaseMessage, frozen=True):
     """Application subscription details"""
 
-    subscriptionToken: str  # Application key identifier
-    expiryDateTime: Optional[Date] = None
-    expiredDateTime: Optional[Date] = None
-    createdDateTime: Optional[Date] = None
-    activationDateTime: Optional[Date] = None
-    cancellationDateTime: Optional[Date] = None
-    subscriptionStatus: Optional[SubscriptionStatus] = None
-    clientReference: Optional[str] = None
-    vendorClientId: Optional[str] = None
+    subscription_token: str  # Application key identifier
+    expiry_date_time: Optional[Date] = None
+    expired_date_time: Optional[Date] = None
+    created_date_time: Optional[Date] = None
+    activation_date_time: Optional[Date] = None
+    cancellation_date_time: Optional[Date] = None
+    subscription_status: Optional[SubscriptionStatus] = None
+    client_reference: Optional[str] = None
+    vendor_client_id: Optional[str] = None
 
 
 class SubscriptionHistory(BaseMessage, frozen=True):
     """Application subscription history details"""
 
-    subscriptionToken: str  # Application key identifier
-    expiryDateTime: Optional[Date] = None
-    expiredDateTime: Optional[Date] = None
-    createdDateTime: Optional[Date] = None
-    activationDateTime: Optional[Date] = None
-    cancellationDateTime: Optional[Date] = None
-    subscriptionStatus: Optional[SubscriptionStatus] = None
-    clientReference: Optional[str] = None
+    subscription_token: str  # Application key identifier
+    expiry_date_time: Optional[Date] = None
+    expired_date_time: Optional[Date] = None
+    created_date_time: Optional[Date] = None
+    activation_date_time: Optional[Date] = None
+    cancellation_date_time: Optional[Date] = None
+    subscription_status: Optional[SubscriptionStatus] = None
+    client_reference: Optional[str] = None
 
 
 class SubscriptionTokenInfo(BaseMessage, frozen=True):
     """Subscription token information"""
 
-    subscriptionToken: str
-    activatedDateTime: Optional[Date] = None
-    expiryDateTime: Optional[Date] = None
-    expiredDateTime: Optional[Date] = None
-    cancellationDateTime: Optional[Date] = None
-    subscriptionStatus: Optional[SubscriptionStatus] = None
+    subscription_token: str
+    activated_date_time: Optional[Date] = None
+    expiry_date_time: Optional[Date] = None
+    expired_date_time: Optional[Date] = None
+    cancellation_date_time: Optional[Date] = None
+    subscription_status: Optional[SubscriptionStatus] = None
 
 
 class AccountSubscription(BaseMessage, frozen=True):
     """Application subscription details"""
 
-    subscriptionTokens: list[SubscriptionTokenInfo]
-    applicationName: Optional[str] = None
-    applicationVersionId: Optional[str] = None
+    subscription_tokens: list[SubscriptionTokenInfo]
+    application_name: Optional[str] = None
+    application_version_id: Optional[str] = None
 
 
 class DeveloperAppVersion(BaseMessage, frozen=True):
     """Describes a version of an external application"""
 
     owner: str  # The user who owns the specific version of the application
-    versionId: int  # The unique Id of the application version
+    version_id: int  # The unique Id of the application version
     version: str  # identifier string such as 1.0, 2.0. Unique for a given application.
-    applicationKey: str  # The unique application key associated with this application version
+    application_key: str  # The unique application key associated with this application version
 
     # Indicates whether the data exposed by platform services as seen by this
     # application key is delayed or realtime.
     delayData: bool
-    subscriptionRequired: bool  # Indicates whether the application version needs explicit subscription
+    subscription_required: bool  # Indicates whether the application version needs explicit subscription
 
     # Indicates whether the application version needs explicit management by the software owner.
     # A value of false indicates, this is a version meant for personal developer use.
-    ownerManaged: bool
+    owner_managed: bool
     active: bool  # Indicates whether the application version is currently active
 
     # Public unique string provided to the Vendor that they can use to pass to the
     # Betfair API in order to identify themselves.
-    vendorId: Optional[str] = None
+    vendor_id: Optional[str] = None
     # Private unique string provided to the Vendor that they pass with certain calls
     # to confirm their identity. Linked to a particular App Key.
-    vendorSecret: Optional[str] = None
+    vendor_secret: Optional[str] = None
 
 
 class DeveloperApp(BaseMessage, frozen=True):
     """Describes developer/vendor specific application"""
 
-    appName: str  # The unique name of the application
-    appId: int  # A unique id of this application
-    appVersions: list[DeveloperAppVersion]  # The application versions (including application keys)
+    app_name: str  # The unique name of the application
+    app_id: int  # A unique id of this application
+    app_versions: list[DeveloperAppVersion]  # The application versions (including application keys)
 
 
 class AccountFundsResponse(BaseMessage, frozen=True):
     """Response for retrieving available to bet."""
 
-    availableToBetBalance: Optional[float] = None
+    available_to_bet_balance: Optional[float] = None
     exposure: Optional[float] = None
-    retainedCommission: Optional[float] = None  # Sum of retained commission.
-    exposureLimit: Optional[float] = None
+    retained_commission: Optional[float] = None  # Sum of retained commission.
+    exposure_limit: Optional[float] = None
 
     # User Discount Rate. Please note: Betfair AUS/NZ customers should not rely on this to determine
     # their discount rates which are now applied at the account level.
-    discountRate: Optional[float] = None
-    pointsBalance: Optional[int] = None
+    discount_rate: Optional[float] = None
+    points_balance: Optional[int] = None
 
     # This is NOT documented in the API description, but seems to be present at least int recorded data
     wallet: Optional[Wallet] = None
 
 
 class AccountDetailsResponse(BaseMessage, frozen=True):
     """Response for Account details."""
 
     # Default user currency Code. See Currency Parameters for minimum bet sizes relating to each currency.
-    currencyCode: Optional[str] = None
-    firstName: Optional[str] = None
-    lastName: Optional[str] = None
-    localeCode: Optional[str] = None
+    currency_code: Optional[str] = None
+    first_name: Optional[str] = None
+    last_name: Optional[str] = None
+    locale_code: Optional[str] = None
 
     # Region based on users zip/postcode (ISO 3166-1 alpha-3 format). Defaults to GBR if
     # zip/postcode cannot be identified.
     region: Optional[str] = None
     timezone: Optional[str] = None  # User Time Zone.
 
     # User Discount Rate.   Please note:  Betfair AUS/NZ customers should not rely on this to
     # determine their discount rates which are now applied at the account level.
-    discountRate: Optional[float] = None
-    pointsBalance: Optional[int] = None  # The Betfair points balance.
-    countryCode: Optional[str] = None  # The customer's country of residence (ISO 2 Char format)
+    discount_rate: Optional[float] = None
+    points_balance: Optional[int] = None  # The Betfair points balance.
+    country_code: Optional[str] = None  # The customer's country of residence (ISO 2 Char format)
 
 
 class StatementLegacyData(BaseMessage, frozen=True):
     """Summary of a cleared order."""
 
-    avgPrice: Optional[float]  # The average matched price of the bet (null if no part has been matched)
+    avg_price: Optional[float]  # The average matched price of the bet (null if no part has been matched)
 
     # The amount of the stake of your bet. (0 for commission payments or deposit/withdrawals)
-    betSize: Optional[float] = None
-    betType: Optional[str] = None  # Back or lay
-    betCategoryType: Optional[str] = None  # Exchange, Market on Close SP bet, or Limit on Close SP bet.
-    commissionRate: Optional[str] = None  # Commission rate on market
-    eventId: Optional[int] = None  # Please note: this is the Id of the market without the associated exchangeId
-    eventTypeId: Optional[int] = None
+    bet_size: Optional[float] = None
+    bet_type: Optional[str] = None  # Back or lay
+    bet_category_type: Optional[str] = None  # Exchange, Market on Close SP bet, or Limit on Close SP bet.
+    commission_rate: Optional[str] = None  # Commission rate on market
+    event_id: Optional[int] = None  # Please note: this is the Id of the market without the associated exchangeId
+    event_type_id: Optional[int] = None
 
     # Full Market Name. For card payment items, this field contains the card name
-    fullMarketName: Optional[str] = None
-    grossBetAmount: Optional[float] = None  # The winning amount to which commission is applied.
+    full_market_name: Optional[str] = None
+    gross_bet_amount: Optional[float] = None  # The winning amount to which commission is applied.
 
     # Market Name. For card transactions, this field indicates the type of card
     # transaction (deposit, deposit fee, or withdrawal).
-    marketName: Optional[str] = None
+    market_name: Optional[str] = None
 
     # Market type. For account deposits and withdrawals, marketType is set to NOT_APPLICABLE.
-    marketType: Optional[str] = None
-    placedDate: Optional[Date] = None  # Date and time of bet placement
+    market_type: Optional[str] = None
+    placed_date: Optional[Date] = None  # Date and time of bet placement
 
     # Id of the selection (this will be the same for the same selection across markets)
-    selectionId: Optional[int] = None
-    selectionName: Optional[str] = None  # Name of the selection
-    startDate: Optional[Date] = None  # Date and time at the bet portion was settled
-    transactionType: Optional[str] = None  # Debit or credit
-    transactionId: Optional[int] = None  # The unique reference Id assigned to account deposit and withdrawals.
-    winLose: Optional[WinLose] = None
+    selection_id: Optional[int] = None
+    selection_name: Optional[str] = None  # Name of the selection
+    start_date: Optional[Date] = None  # Date and time at the bet portion was settled
+    transaction_type: Optional[str] = None  # Debit or credit
+    transaction_id: Optional[int] = None  # The unique reference Id assigned to account deposit and withdrawals.
+    win_lose: Optional[WinLose] = None
 
     # In the instance of a dead heat, this field will indicate the number of winners
     # involved in the dead heat (null otherwise)
-    deadHeatPriceDivisor: Optional[float] = None
+    dead_heat_price_divisor: Optional[float] = None
 
     # Currently returns same value as avgPrice. Once released will display the average matched
     # price of the bet with no rounding applied
-    avgPriceRaw: Optional[float] = None
+    avg_price_raw: Optional[float] = None
 
 
 class StatementItem(BaseMessage, kw_only=True, frozen=True):
     """Summary of a cleared order."""
 
     # An external reference, eg. equivalent to betId in the case of an exchange bet statement item.
-    refId: Optional[str] = None
+    ref_id: Optional[str] = None
 
     # The date and time of the statement item, eg. equivalent to settledData for an exchange
     # bet statement item. (in ISO-8601 format, not translated)
-    itemDate: Date
+    item_date: Date
     amount: Optional[float] = None  # The amount of money the balance is adjusted by
     balance: Optional[float] = None
 
     # Class of statement item. This value will determine which set of keys will be included in itemClassData
-    itemClass: Optional[ItemClass] = None
+    item_class: Optional[ItemClass] = None
     # Key value pairs describing the current statement item. The set of keys will be
     # determined by the itemClass
-    itemClassData: Optional[dict[str, str]] = None
+    item_class_data: Optional[dict[str, str]] = None
     # Set of fields originally returned from APIv6. Provided to facilitate migration from
     # APIv6 to API-NG, and ultimately onto itemClass and itemClassData
-    legacyData: Optional[StatementLegacyData] = None
+    legacy_data: Optional[StatementLegacyData] = None
 
 
 class AccountStatementReport(BaseMessage, frozen=True):
     """A container representing search results."""
 
-    accountStatement: list[StatementItem]  # The list of statement items returned by your request.
-    moreAvailable: bool  # Indicates whether there are further result items beyond this page.
+    account_statement: list[StatementItem]  # The list of statement items returned by your request.
+    more_available: bool  # Indicates whether there are further result items beyond this page.
 
 
 class CurrencyRate(BaseMessage, frozen=True):
-    currencyCode: Optional[str] = None  # Three-letter ISO 4217 code
+    currency_code: Optional[str] = None  # Three-letter ISO 4217 code
     rate: Optional[float] = None  # Exchange rate for the currency specified in the request
 
 
 class AuthorisationResponse(BaseMessage, frozen=True):
     """Wrapper object containing authorisation code and redirect URL for web vendors"""
 
-    authorisationCode: str  # The authorisation code
-    redirectUrl: str  # URL to redirect the user to the vendor page
+    authorisation_code: str  # The authorisation code
+    redirect_url: str  # URL to redirect the user to the vendor page
 
 
-class SubscriptionOptions(BaseMessage, frozen=True):
+class SubscriptionOptions(BaseMessage, frozen=True, rename=None):
+    # No rename: SubscriptionOption fields don't use camelCase in Betfair API
+
     """Wrapper object containing details of how a subscription should be created"""
 
     # How many days should a created subscription last for. Open-ended subscription created
     # if value not provided. Relevant only if createdSubscription is true.
     subscription_length: Optional[int] = None
 
     # An existing subscription token that the caller wishes to be activated instead of creating a new one.
     # Ignored is createSubscription is true.
     subscription_token: Optional[str] = None
     client_reference: Optional[str] = None  # Any client reference for this subscription token request.
 
 
-class VendorAccessTokenInfo(BaseMessage, frozen=True):
+class VendorAccessTokenInfo(BaseMessage, frozen=True, rename=None):
+    # No rename: VendorAccessTokenInfo fields don't use camelCase in Betfair API
+
     """
     Wrapper object containing UserVendorSessionToken, RefreshToken and
     optionally a Subscription Token if one was created
     """
 
     access_token: str  # Session token used by web vendors
     token_type: TokenType  # Type of the token
@@ -239,17 +243,17 @@
     # Object containing the vendor client id and optionally some subscription information
     application_subscription: ApplicationSubscription
 
 
 class VendorDetails(BaseMessage, frozen=True):
     """Wrapper object containing vendor name and redirect url"""
 
-    appVersionId: int  # Internal id of the application
-    vendorName: str
-    redirectUrl: Optional[str] = None  # URL to be redirected to
+    app_version_id: int  # Internal id of the application
+    vendor_name: str
+    redirect_url: Optional[str] = None  # URL to be redirected to
 
 
 class AffiliateRelation(BaseMessage, frozen=True):
     """Wrapper object containing affiliate relation details"""
 
-    vendorClientId: str  # ID of user
     status: AffiliateRelationStatus
+    vendor_client_id: str  # ID of user
```

### Comparing `betfair_parser-0.2.2/betfair_parser/spec/betting/enums.py` & `betfair_parser-0.2.3/betfair_parser/spec/betting/enums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.2/betfair_parser/spec/betting/listings.py` & `betfair_parser-0.2.3/betfair_parser/spec/betting/listings.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,108 +20,108 @@
     PriceProjection,
     TimeRangeResult,
     VenueResult,
 )
 from betfair_parser.spec.common import BaseMessage, BetId, Date, MarketId, Request, Response, SelectionId
 
 
-class ListingParams(BaseMessage, frozen=True):
+class _ListingParams(BaseMessage, frozen=True):
     filter: MarketFilter
     locale: Optional[str] = None
 
 
-class listCompetitions(Request, kw_only=True, frozen=True):
+class ListCompetitions(Request, kw_only=True, frozen=True):
     """
     Returns a list of Competitions (i.e., World Cup 2013) associated with the markets selected by
     the MarketFilter. Currently only Football markets have an associated competition.
     """
 
     method = "SportsAPING/v1.0/listCompetitions"
-    params: ListingParams
+    params: _ListingParams
     return_type = Response[list[CompetitionResult]]
 
 
-class listCountries(Request, kw_only=True, frozen=True):
+class ListCountries(Request, kw_only=True, frozen=True):
     """
     Returns a list of Countries associated with the markets selected by the MarketFilter.
     """
 
     method = "SportsAPING/v1.0/listCountries"
-    params: ListingParams
+    params: _ListingParams
     return_type = Response[list[CountryCodeResult]]
 
 
-class listEvents(Request, kw_only=True, frozen=True):
+class ListEvents(Request, kw_only=True, frozen=True):
     """
     Returns a list of Events (i.e, Reading vs. Man United) associated with the markets selected
     by the MarketFilter.
     """
 
     method = "SportsAPING/v1.0/listEvents"
-    params: ListingParams
+    params: _ListingParams
     return_type = Response[list[EventResult]]
 
 
-class listEventTypes(Request, kw_only=True, frozen=True):
+class ListEventTypes(Request, kw_only=True, frozen=True):
     """
     Returns a list of Event Types (i.e. Sports) associated with the markets selected by the
     MarketFilter.
     """
 
     method = "SportsAPING/v1.0/listEventTypes"
-    params: ListingParams
+    params: _ListingParams
     return_type = Response[list[EventTypeResult]]
 
 
-class listMarketTypes(Request, kw_only=True, frozen=True):
+class ListMarketTypes(Request, kw_only=True, frozen=True):
     """
     Returns a list of market types (i.e. MATCH_ODDS, NEXT_GOAL) associated with the markets selected
     by the MarketFilter. The market types are always the same, regardless of locale.
     """
 
     method = "SportsAPING/v1.0/listMarketTypes"
-    params: ListingParams
+    params: _ListingParams
     return_type = Response[list[MarketTypeResult]]
 
 
-class listVenues(Request, kw_only=True, frozen=True):
+class ListVenues(Request, kw_only=True, frozen=True):
     """
     Returns a list of Venues (i.e. Cheltenham, Ascot) associated with the markets selected by the
     MarketFilter. Currently, only Horse Racing markets are associated with a Venue.
     """
 
     method = "SportsAPING/v1.0/listVenues"
-    params: ListingParams
+    params: _ListingParams
     return_type = Response[list[VenueResult]]
 
 
 # More complex listings
 
 
-class listMarketBookParams(BaseMessage, frozen=True):
-    marketIds: list[str]  # One or more market ids
-    priceProjection: Optional[
+class _ListMarketBookParams(BaseMessage, frozen=True):
+    market_ids: list[str]  # One or more market ids
+    price_projection: Optional[
         PriceProjection
     ] = None  # The projection of price data you want to receive in the response
-    orderProjection: Optional[OrderProjection] = None  # The orders you want to receive in the response
-    matchProjection: Optional[MatchProjection] = None  # If you ask for orders, specifies the representation of matches
-    includeOverallPosition: Optional[bool] = None  # If you ask for orders, returns matches for each selection
-    partitionMatchedByStrategyRef: Optional[
+    order_projection: Optional[OrderProjection] = None  # The orders you want to receive in the response
+    match_projection: Optional[MatchProjection] = None  # If you ask for orders, specifies the representation of matches
+    include_overall_position: Optional[bool] = None  # If you ask for orders, returns matches for each selection
+    partition_matched_by_strategy_ref: Optional[
         bool
     ] = None  # Returns the breakdown of matches by strategy for each selection
-    customerStrategyRefs: Optional[set[str]] = None
-    currencyCode: Optional[str] = None  # A Betfair standard currency code
+    customer_strategy_refs: Optional[set[str]] = None
+    currency_code: Optional[str] = None  # A Betfair standard currency code
     locale: Optional[str] = None  # The language used for the response
-    matchedSince: Optional[
+    matched_since: Optional[
         Date
     ] = None  # Restricts to orders with at least one fragment matched since the specified date
-    betIds: Optional[set[BetId]] = None  # Restricts to orders with the specified bet IDs
+    bet_ids: Optional[set[BetId]] = None  # Restricts to orders with the specified bet IDs
 
 
-class listMarketBook(Request, kw_only=True, frozen=True):
+class ListMarketBook(Request, kw_only=True, frozen=True):
     """
     Returns a list of dynamic data about markets. Dynamic data includes prices, the status of the
     market, the status of selections, the traded volume, and the status of any orders you have
     placed in the market.
 
     Please note: Separate requests should be made for OPEN & CLOSED markets. Request that include
     both OPEN & CLOSED markets will only return those markets that are OPEN.
@@ -134,93 +134,95 @@
     The level of matched volume aggregation (MatchProjection) requested should be
     ROLLED_UP_BY_AVG_PRICE or ROLLED_UP_BY_PRICE, the former being preferred. This provides a single
     call in which you can track prices, traded volume, unmatched orders and your evolving matched
     position with a reasonably fixed, minimally sized response.
     """
 
     method = "SportsAPING/v1.0/listMarketBook"
-    params: listMarketBookParams
+    params: _ListMarketBookParams
     return_type = Response[list[MarketBook]]
 
 
-class listMarketCatalogueParams(BaseMessage, kw_only=True, frozen=True):
+class _ListMarketCatalogueParams(BaseMessage, kw_only=True, frozen=True):
     filter: MarketFilter  # The filter to select desired markets
-    marketProjection: Optional[set[MarketProjection]] = None  # The type and amount of data returned about the market
+    market_projection: Optional[set[MarketProjection]] = None  # The type and amount of data returned about the market
     sort: Optional[MarketSort] = None  # The order of the results, defaults to RANK
-    maxResults: int  # Limit on the total number of results returned
+    max_results: int  # Limit on the total number of results returned
     locale: Optional[str] = None  # The language used for the response
 
 
-class listMarketCatalogue(Request, kw_only=True, frozen=True):
+class ListMarketCatalogue(Request, kw_only=True, frozen=True):
     """
     Returns a list of information about published (ACTIVE/SUSPENDED) markets that does not change
     (or changes very rarely). You use listMarketCatalogue to retrieve the name of the market, the
     names of selections and other information about markets.  Market Data Request Limits apply to
     requests made to listMarketCatalogue.
 
     Please note: listMarketCatalogue does not return markets that are CLOSED.
     """
 
     method = "SportsAPING/v1.0/listMarketCatalogue"
-    params: listMarketCatalogueParams
+    params: _ListMarketCatalogueParams
     return_type = Response[list[MarketCatalogue]]
 
 
-class listMarketProfitAndLossParams(BaseMessage, frozen=True):
-    marketIds: set[MarketId]  # List of markets to calculate profit and loss
-    includeSettledBets: Optional[bool] = False  # Option to include settled bets (partially settled markets only)
-    includeBspBets: Optional[bool] = False  # Option to include BSP bets
-    netOfCommission: Optional[bool] = False  # Option to return profit and loss net of users current commission rate
+class _ListMarketProfitAndLossParams(BaseMessage, frozen=True):
+    market_ids: set[MarketId]  # List of markets to calculate profit and loss
+    include_settled_bets: Optional[bool] = False  # Option to include settled bets (partially settled markets only)
+    include_bsp_bets: Optional[bool] = False  # Option to include BSP bets
+    net_of_commission: Optional[bool] = False  # Option to return profit and loss net of users current commission rate
 
 
-class listMarketProfitAndLoss(Request, kw_only=True, frozen=True):
+class ListMarketProfitAndLoss(Request, kw_only=True, frozen=True):
     """Returns a list of Countries associated with the markets selected by the MarketFilter."""
 
     method = "SportsAPING/v1.0/listMarketProfitAndLoss"
-    params: listMarketProfitAndLossParams
+    params: _ListMarketProfitAndLossParams
     return_type = Response[list[MarketProfitAndLoss]]
 
 
-class listRunnerBookParams(BaseMessage, frozen=True):
-    marketId: MarketId  # The unique id for the market
-    selectionId: SelectionId  # The unique id for the selection in the market
+class _ListRunnerBookParams(BaseMessage, frozen=True):
+    market_id: MarketId  # The unique id for the market
+    selection_id: SelectionId  # The unique id for the selection in the market
     handicap: Optional[float] = None  # The handicap associated with the runner in case of Asian handicap market
-    priceProjection: Optional[PriceProjection] = None
-    orderProjection: Optional[OrderProjection] = None
-    matchProjection: Optional[MatchProjection] = None  # If you ask for orders, specifies the representation of matches
-    includeOverallPosition: Optional[bool] = None  # If you ask for orders, returns matches for each selection
-    partitionMatchedByStrategyRef: Optional[bool] = None  # Return a breakdown of matches by strategy for each selection
-    customerStrategyRefs: Optional[set[str]] = None
-    currencyCode: Optional[str] = None  # A Betfair standard currency code
+    price_projection: Optional[PriceProjection] = None
+    order_projection: Optional[OrderProjection] = None
+    match_projection: Optional[MatchProjection] = None  # If you ask for orders, specifies the representation of matches
+    include_overall_position: Optional[bool] = None  # If you ask for orders, returns matches for each selection
+    partition_matched_by_strategy_ref: Optional[
+        bool
+    ] = None  # Return a breakdown of matches by strategy for each selection
+    customer_strategy_refs: Optional[set[str]] = None
+    currency_code: Optional[str] = None  # A Betfair standard currency code
     locale: Optional[str] = None  # The language used for the response
-    matchedSince: Optional[Date] = None  # Restricts to orders with at least one fragment matched since specified date
-    betIds: Optional[set[BetId]] = None  # Restricts to orders with the specified bet IDs
+    matched_since: Optional[Date] = None  # Restricts to orders with at least one fragment matched since specified date
+    bet_ids: Optional[set[BetId]] = None  # Restricts to orders with the specified bet IDs
 
 
-class listRunnerBook(Request, kw_only=True, frozen=True):
+class ListRunnerBook(Request, kw_only=True, frozen=True):
     """
     Returns a list of dynamic data about a market and a specified runner. Dynamic data includes
     prices, the status of the market, the status of selections, the traded volume, and the status
     of any orders you have placed in the market..
     """
 
     method = "SportsAPING/v1.0/listRunnerBook"
-    params: listRunnerBookParams
+    params: _ListRunnerBookParams
     return_type = Response[list[MarketBook]]
 
 
-class listTimeRangesParams(BaseMessage, frozen=True):
+class _ListTimeRangesParams(BaseMessage, frozen=True):
     # The filter to select desired markets. All markets that match the criteria in the filter are selected.
     filter: MarketFilter
     # The granularity of time periods that correspond to markets selected by the market filter.
     granularity: TimeGranularity
 
 
-class listTimeRanges(Request, kw_only=True, frozen=True):
+class ListTimeRanges(Request, kw_only=True, frozen=True):
     """
     Returns a list of time ranges in the granularity specified in the request (i.e. 3PM to 4PM,
     Aug 14th to Aug 15th) associated with the markets selected by the MarketFilter.
     """
 
     method = "SportsAPING/v1.0/listTimeRanges"
-    params: listTimeRangesParams
+    params: _ListTimeRangesParams
     return_type = Response[list[TimeRangeResult]]
```

### Comparing `betfair_parser-0.2.2/betfair_parser/spec/betting/orders.py` & `betfair_parser-0.2.3/betfair_parser/spec/betting/orders.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,142 +28,142 @@
     MarketId,
     Request,
     Response,
     TimeRange,
 )
 
 
-class placeOrdersParams(BaseMessage, frozen=True):
-    marketId: str
+class _PlaceOrdersParams(BaseMessage, frozen=True):
+    market_id: str
     instructions: list[PlaceInstruction]
-    customerRef: Optional[CustomerRef] = None
-    marketVersion: Optional[MarketVersion] = None
-    customerStrategyRef: Optional[CustomerStrategyRef] = None
+    customer_ref: Optional[CustomerRef] = None
+    market_version: Optional[MarketVersion] = None
+    customer_strategy_ref: Optional[CustomerStrategyRef] = None
     async_: Optional[bool] = msgspec.field(name="async", default=False)
 
 
-class placeOrders(Request, kw_only=True, frozen=True):
+class PlaceOrders(Request, kw_only=True, frozen=True):
     """Place new orders into market.
 
     Please note that additional bet sizing rules apply to bets placed into the Italian Exchange.
 
     In normal circumstances the placeOrders is an atomic operation. PLEASE NOTE: if the
     'Best Execution' features is switched off, placeOrders can return ‘PROCESSED_WITH_ERRORS’
     meaning that some bets can be rejected and other placed when submitted in the same
     PlaceInstruction.
     """
 
     method = "SportsAPING/v1.0/placeOrders"
-    params: placeOrdersParams
+    params: _PlaceOrdersParams
     return_type = Response[PlaceExecutionReport]
 
 
-class cancelOrdersParams(BaseMessage, frozen=True):
-    marketId: Optional[str] = None
+class _CancelOrdersParams(BaseMessage, frozen=True):
+    market_id: Optional[str] = None
     instructions: Optional[list[CancelInstruction]] = None
-    customerRef: Optional[CustomerRef] = None
+    customer_ref: Optional[CustomerRef] = None
 
 
-class cancelOrders(Request, kw_only=True, frozen=True):
+class CancelOrders(Request, kw_only=True, frozen=True):
     """
     Cancel all bets OR cancel all bets on a market OR fully or partially cancel particular
     orders on a market. Only LIMIT orders can be cancelled or partially cancelled once placed.
     """
 
     method = "SportsAPING/v1.0/cancelOrders"
-    params: cancelOrdersParams
+    params: _CancelOrdersParams
     return_type = Response[CancelExecutionReport]
 
 
-class replaceOrdersParams(BaseMessage, frozen=True):
-    marketId: str
+class _ReplaceOrdersParams(BaseMessage, frozen=True):
+    market_id: str
     instructions: list[ReplaceInstruction]
-    customerRef: Optional[CustomerRef] = None
-    marketVersion: Optional[MarketVersion] = None
+    customer_ref: Optional[CustomerRef] = None
+    market_version: Optional[MarketVersion] = None
     async_: Optional[bool] = msgspec.field(name="async", default=False)
 
 
-class replaceOrders(Request, kw_only=True, frozen=True):
+class ReplaceOrders(Request, kw_only=True, frozen=True):
     """
     This operation is logically a bulk cancel followed by a bulk place. The cancel is completed
     first then the new orders are placed. The new orders will be placed atomically in that they
     will all be placed or none will be placed. In the case where the new orders cannot be placed
     the cancellations will not be rolled back. See ReplaceInstruction.
     """
 
     method = "SportsAPING/v1.0/replaceOrders"
-    params: replaceOrdersParams
+    params: _ReplaceOrdersParams
     return_type = Response[ReplaceExecutionReport]
 
 
-class listClearedOrdersParams(BaseMessage, frozen=True):
-    betStatus: BetStatus  # Restricts the results to the specified status.
-    eventTypeIds: Optional[set[EventTypeId]] = None  # Restricts the results to the specified Event Type IDs.
-    eventIds: Optional[set[EventId]] = None  # Restricts the results to the specified Event IDs.
-    marketIds: Optional[set[MarketId]] = None  # Restricts the results to the specified market IDs.
-    runnerIds: Optional[set[RunnerId]] = None  # Restricts the results to the specified Runners.
-    betIds: Optional[set[BetId]] = None  # Restricts the results to the specified bet IDs, maximum 1000 betIds
-    customerOrderRefs: Optional[set[CustomerOrderRef]] = None
-    customerStrategyRefs: Optional[set[CustomerStrategyRef]] = None
+class _ListClearedOrdersParams(BaseMessage, frozen=True):
+    bet_status: BetStatus  # Restricts the results to the specified status.
+    event_type_ids: Optional[set[EventTypeId]] = None  # Restricts the results to the specified Event Type IDs.
+    event_ids: Optional[set[EventId]] = None  # Restricts the results to the specified Event IDs.
+    market_ids: Optional[set[MarketId]] = None  # Restricts the results to the specified market IDs.
+    runner_ids: Optional[set[RunnerId]] = None  # Restricts the results to the specified Runners.
+    bet_ids: Optional[set[BetId]] = None  # Restricts the results to the specified bet IDs, maximum 1000 betIds
+    customer_order_refs: Optional[set[CustomerOrderRef]] = None
+    customer_strategy_refs: Optional[set[CustomerStrategyRef]] = None
     side: Optional[Side] = None  # Restricts the results to the specified side.
 
     # Optionally restricts the results to be from/to the specified settled date. This date is inclusive,
     # i.e. if an order was cleared on exactly this date (to the millisecond) then it will be included
     # in the results. If the from is later than the to, no results will be returned.
     # Please Note: if you have a longer running market that is settled at multiple different times
     # then there is no way to get the returned market rollup to only include bets settled in a certain
     # date range, it will always return the overall position from the market including all settlements.
-    settledDateRange: Optional[TimeRange] = None
+    settled_date_range: Optional[TimeRange] = None
 
     # If not supplied then the lowest level is returned, i.e. bet by bet This is only applicable to SETTLED BetStatus.
-    groupBy: Optional[GroupBy] = None
-    includeItemDescription: Optional[bool] = None
+    group_by: Optional[GroupBy] = None
+    include_item_description: Optional[bool] = None
     locale: Optional[str] = None  # The language used for the itemDescription, defaults to account settings
-    fromRecord: Optional[int] = None  # Specifies the first record that will be returned. Records start at index zero.
-    recordCount: Optional[int] = None  # Number of records from the index position 'fromRecord', maximum 1000
+    from_record: Optional[int] = None  # Specifies the first record that will be returned. Records start at index zero.
+    record_count: Optional[int] = None  # Number of records from the index position 'fromRecord', maximum 1000
 
 
-class listClearedOrders(Request, kw_only=True, frozen=True):
+class ListClearedOrders(Request, kw_only=True, frozen=True):
     """
     Returns a list of settled bets based on the bet status, ordered by settled date. To retrieve
     more than 1000 records, you need to make use of the fromRecord and recordCount parameters.
 
     By default the service will return all available data for the last 90 days (see Best Practice
     note below).  The fields available at each roll-up are available here
 
     Best Practice:
     You should specify a settledDateRange "from" date when making requests for data. This reduces
     the amount of data that requires downloading & improves the speed of the response. Specifying
     a "from" date of the last call will ensure that only new data is returned.
     """
 
     method = "SportsAPING/v1.0/listClearedOrders"
-    params: listClearedOrdersParams
+    params: _ListClearedOrdersParams
     return_type = Response[ClearedOrderSummaryReport]
 
 
-class listCurrentOrdersParams(BaseMessage, frozen=True):
+class _ListCurrentOrdersParams(BaseMessage, frozen=True):
     """
     Parameters for retrieving a list of current orders.
     """
 
-    betIds: Optional[set[BetId]] = None  # Restricts the results to the specified bet IDs
-    marketIds: Optional[set[str]] = None  # Restricts the results to the specified market IDs
-    orderProjection: Optional[OrderProjection] = None  # Restricts the results to the specified order status
-    customerOrderRefs: Optional[set[CustomerOrderRef]] = None
-    customerStrategyRefs: Optional[set[CustomerStrategyRef]] = None
-    dateRange: Optional[TimeRange] = None  # Restricts the results to be from/to the specified date
-    orderBy: Optional[OrderBy] = None  # Specifies how the results will be ordered
-    sortDir: Optional[SortDir] = None  # Specifies the direction the results will be sorted in
-    fromRecord: Optional[int] = None  # Specifies the first record that will be returned
-    recordCount: Optional[int] = None  # Specifies how many records will be returned
-    includeItemDescription: Optional[bool] = None
+    bet_ids: Optional[set[BetId]] = None  # Restricts the results to the specified bet IDs
+    market_ids: Optional[set[str]] = None  # Restricts the results to the specified market IDs
+    order_projection: Optional[OrderProjection] = None  # Restricts the results to the specified order status
+    customer_order_refs: Optional[set[CustomerOrderRef]] = None
+    customer_strategy_refs: Optional[set[CustomerStrategyRef]] = None
+    date_range: Optional[TimeRange] = None  # Restricts the results to be from/to the specified date
+    order_by: Optional[OrderBy] = None  # Specifies how the results will be ordered
+    sort_dir: Optional[SortDir] = None  # Specifies the direction the results will be sorted in
+    from_record: Optional[int] = None  # Specifies the first record that will be returned
+    record_count: Optional[int] = None  # Specifies how many records will be returned
+    include_item_description: Optional[bool] = None
 
 
-class listCurrentOrders(Request, kw_only=True, frozen=True):
+class ListCurrentOrders(Request, kw_only=True, frozen=True):
     """
     Returns a list of your current orders. Optionally you can filter and sort your current orders
     using the various parameters, setting none of the parameters will return all of your current
     orders up to a maximum of 1000 bets, ordered BY_BET and sorted EARLIEST_TO_LATEST. To retrieve
     more than 1000 orders, you need to make use of the fromRecord and recordCount parameters.
 
     Best Practice:
@@ -171,23 +171,23 @@
     the dateRange, orderBy "BY_MATCH_TIME" and orderProjection “ALL” to filter fully/partially matched
     orders from the list of returned bets. The response will then filter out any bet records that
     have no matched date and provide a list of betIds in the order which they are fully/partially
     matched from the date and time specified in the dateRange field.
     """
 
     method = "SportsAPING/v1.0/listCurrentOrders"
-    params: listCurrentOrdersParams
+    params: _ListCurrentOrdersParams
     return_type = Response[CurrentOrderSummaryReport]
 
 
-class updateOrdersParams(BaseMessage, frozen=True):
-    marketId: str  # The market id these orders are to be placed on
+class _UpdateOrdersParams(BaseMessage, frozen=True):
+    market_id: str  # The market id these orders are to be placed on
     instructions: list[UpdateInstruction]  # The limit of update instructions per request is 60
-    customerRef: Optional[CustomerRef] = None
+    customer_ref: Optional[CustomerRef] = None
 
 
-class updateOrders(Request, kw_only=True, frozen=True):
+class UpdateOrders(Request, kw_only=True, frozen=True):
     """Update non-exposure changing fields."""
 
     method = "SportsAPING/v1.0/updateOrders"
-    params: updateOrdersParams
+    params: _UpdateOrdersParams
     return_type = Response[UpdateExecutionReport]
```

### Comparing `betfair_parser-0.2.2/betfair_parser/spec/betting/type_definitions.py` & `betfair_parser-0.2.3/betfair_parser/spec/betting/type_definitions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Optional
 
+import msgspec
+
 from betfair_parser.spec.betting.enums import (
     BetTargetType,
     ExecutionReportErrorCode,
     ExecutionReportStatus,
     InstructionReportErrorCode,
     InstructionReportStatus,
     MarketBettingType,
@@ -44,561 +46,551 @@
 class Competition(BaseMessage, frozen=True):
     id: Optional[CompetitionId] = None
     name: Optional[str] = None
 
 
 class CompetitionResult(BaseMessage, frozen=True):
     competition: Optional[Competition] = None
-    marketCount: Optional[int] = None  # Count of markets associated with this competition
-    competitionRegion: Optional[str] = None  # Region in which this competition is happening
+    market_count: Optional[int] = None  # Count of markets associated with this competition
+    competition_region: Optional[str] = None  # Region in which this competition is happening
 
 
 class Event(BaseMessage, frozen=True):
     id: Optional[EventId] = None  # The unique id for the event
     name: Optional[str] = None  # The name of the event
-    countryCode: Optional[CountryCode] = None  # The ISO-2 code for the event, defaults to GB
+    country_code: Optional[CountryCode] = None  # The ISO-2 code for the event, defaults to GB
     timezone: Optional[str] = None  # The timezone in which the event is taking place
     venue: Optional[str] = None
-    openDate: Optional[Date] = None  # The scheduled start date and time of the event
+    open_date: Optional[Date] = None  # The scheduled start date and time of the event
 
 
 class EventResult(BaseMessage, frozen=True):
     event: Optional[Event] = None
-    marketCount: Optional[int] = None  # Count of markets associated with this event
+    market_count: Optional[int] = None  # Count of markets associated with this event
 
 
 class EventType(BaseMessage, frozen=True):
     id: Optional[EventTypeId] = None
     name: Optional[str] = None
 
 
 class EventTypeResult(BaseMessage, frozen=True):
-    eventType: Optional[EventType] = None  # The ID identifying the Event Type
-    marketCount: Optional[int] = None  # Count of markets associated with this eventType
+    event_type: Optional[EventType] = None  # The ID identifying the Event Type
+    market_count: Optional[int] = None  # Count of markets associated with this eventType
 
 
 class MarketTypeResult(BaseMessage, frozen=True):
-    marketType: Optional[str] = None
-    marketCount: Optional[int] = None  # Count of markets associated with this marketType
+    market_type: Optional[str] = None
+    market_count: Optional[int] = None  # Count of markets associated with this marketType
 
 
 class CountryCodeResult(BaseMessage, frozen=True):
-    countryCode: Optional[CountryCode] = None  # The ISO-2 code for the event
-    marketCount: Optional[int] = None  # Count of markets associated with this Country Code
+    country_code: Optional[CountryCode] = None  # The ISO-2 code for the event
+    market_count: Optional[int] = None  # Count of markets associated with this Country Code
 
 
 class VenueResult(BaseMessage, frozen=True):
     venue: Optional[Venue] = None
-    marketCount: Optional[int] = None  # Count of markets associated with this Venue
+    market_count: Optional[int] = None  # Count of markets associated with this Venue
 
 
 class PriceSize(BaseMessage, frozen=True):
     price: Price  # Available price
     size: Size  # Available stake
 
 
 class TimeRangeResult(BaseMessage, frozen=True):
-    timeRange: Optional[TimeRange] = None
-    marketCount: Optional[int] = None  # Count of markets associated with this TimeRange
+    time_range: Optional[TimeRange] = None
+    market_count: Optional[int] = None  # Count of markets associated with this TimeRange
 
 
 class MarketFilter(BaseMessage, frozen=True):
-    textQuery: Optional[str] = None  # Restrict markets by any text associated with the Event name
-    exchangeIds: Optional[set[ExchangeId]] = None  # DEPRECATED
-    eventTypeIds: Optional[set[EventTypeId]] = None  # Restrict markets by event type associated with the market
-    eventIds: Optional[set[EventId]] = None  # Restrict markets by the event id associated with the market
-    competitionIds: Optional[
+    text_query: Optional[str] = None  # Restrict markets by any text associated with the Event name
+    exchange_ids: Optional[set[ExchangeId]] = None  # DEPRECATED
+    event_type_ids: Optional[set[EventTypeId]] = None  # Restrict markets by event type associated with the market
+    event_ids: Optional[set[EventId]] = None  # Restrict markets by the event id associated with the market
+    competition_ids: Optional[
         set[CompetitionId]
     ] = None  # Restrict markets by the competitions associated with the market
-    marketIds: Optional[set[MarketId]] = None  # Restrict markets by the market id associated with the market
+    market_ids: Optional[set[MarketId]] = None  # Restrict markets by the market id associated with the market
     venues: Optional[set[Venue]] = None  # Restrict markets by the venue associated with the market
-    bspOnly: Optional[bool] = None  # Restrict to bsp markets only if True or non-bsp markets if False
+    bsp_only: Optional[bool] = None  # Restrict to bsp markets only if True or non-bsp markets if False
 
     # Restrict to markets that will turn in play if True or will not turn in play if False
-    turnInPlayEnabled: Optional[bool] = None
+    turn_in_play_enabled: Optional[bool] = None
 
     # Restrict to markets that are currently in play if True or are not currently in play if False
-    inPlayOnly: Optional[bool] = None
-    marketBettingTypes: Optional[
-        set[MarketBettingType]
-    ] = None  # Restrict to markets that match the betting type of the market
-    marketCountries: Optional[
-        set[CountryCode]
-    ] = None  # Restrict to markets that are in the specified country or countries
-    marketTypeCodes: Optional[set[str]] = None  # Restrict to markets that match the type of the market
-    marketStartTime: Optional[TimeRange] = None  # Restrict to markets with a market start time range
-    withOrders: Optional[set[str]] = None  # Restrict to markets that I have one or more orders in these status
-    raceTypes: Optional[set[str]] = None  # Restrict by race type
+    in_play_only: Optional[bool] = None
+    market_betting_types: Optional[set[MarketBettingType]] = None  # Match the betting type of the market
+    market_countries: Optional[set[CountryCode]] = None  # Match the specified country or countries
+    market_type_codes: Optional[set[str]] = None  # Restrict to markets that match the type of the market
+    market_start_time: Optional[TimeRange] = None  # Restrict to markets with a market start time range
+    with_orders: Optional[set[str]] = None  # Restrict to markets that I have one or more orders in these status
+    race_types: Optional[set[str]] = None  # Restrict by race type
 
 
 class MarketLineRangeInfo(BaseMessage, frozen=True):
     """Market Line and Range Info"""
 
-    maxUnitValue: float  # Maximum value for the outcome, in market units
-    minUnitValue: float  # Minimum value for the outcome, in market units
+    max_unit_value: float  # Maximum value for the outcome, in market units
+    min_unit_value: float  # Minimum value for the outcome, in market units
     interval: float  # The odds ladder increment interval
-    marketUnit: str  # The type of unit the lines are incremented in
+    market_unit: str  # The type of unit the lines are incremented in
 
 
 class PriceLadderDescription(BaseMessage, frozen=True):
     """Description of the price ladder type and any related data"""
 
     type: PriceLadderType
 
 
 class StartingPrices(BaseMessage, frozen=True):
     """Information about the Betfair Starting Price. Only available in BSP markets"""
 
-    nearPrice: Optional[float] = None  # What the starting price would be if the market was reconciled now
-    farPrice: Optional[float] = None  # What the starting price would be if the market was reconciled now
+    near_price: Optional[float] = None  # What the starting price would be if the market was reconciled now
+    far_price: Optional[float] = None  # What the starting price would be if the market was reconciled now
 
     # The total amount of back bets matched at the actual Betfair Starting Price
-    backStakeTaken: Optional[list[PriceSize]] = None
-    layLiabilityTaken: Optional[list[PriceSize]] = None  # The lay amount matched at the actual Betfair Starting Price
-    actualSP: Optional[float] = None  # The final BSP price for this runner
+    back_stake_taken: Optional[list[PriceSize]] = None
+    lay_liability_taken: Optional[list[PriceSize]] = None  # The lay amount matched at the actual Betfair Starting Price
+    actual_sp: Optional[float] = msgspec.field(name="actualSP", default=None)  # The final BSP price for this runner
 
 
 class ExchangePrices(BaseMessage, frozen=True):
-    availableToBack: Optional[list[PriceSize]] = None
-    availableToLay: Optional[list[PriceSize]] = None
-    tradedVolume: Optional[list[PriceSize]] = None
+    available_to_back: Optional[list[PriceSize]] = None
+    available_to_lay: Optional[list[PriceSize]] = None
+    traded_volume: Optional[list[PriceSize]] = None
 
 
 class Order(BaseMessage, frozen=True):
-    betId: BetId
-    orderType: OrderType
+    bet_id: BetId
+    order_type: OrderType
     status: OrderStatus
-    persistenceType: PersistenceType
+    persistence_type: PersistenceType
     side: Side  # Side (BACK or LAY)
     price: Price
     size: Size
-    bspLiability: Size  # Liability of a given BSP bet
-    placedDate: Date  # Date and time the bet was placed
-    avgPriceMatched: Optional[Price] = None  # Average price matched at
-    sizeMatched: Optional[Size] = None  # Current amount of this bet that was matched
-    sizeRemaining: Optional[Size] = None  # Current amount of this bet that is unmatched
-    sizeLapsed: Optional[Size] = None  # Current amount of this bet that was lapsed
-    sizeCancelled: Optional[Size] = None  # Current amount of this bet that was cancelled
-    sizeVoided: Optional[Size] = None  # Current amount of this bet that was voided
-    customerOrderRef: Optional[CustomerOrderRef] = None  # Customer Order Reference
-    customerStrategyRef: Optional[CustomerStrategyRef] = None  # Customer Strategy Reference
+    bsp_liability: Size  # Liability of a given BSP bet
+    placed_date: Date  # Date and time the bet was placed
+    avg_price_matched: Optional[Price] = None  # Average price matched at
+    size_matched: Optional[Size] = None  # Current amount of this bet that was matched
+    size_remaining: Optional[Size] = None  # Current amount of this bet that is unmatched
+    size_lapsed: Optional[Size] = None  # Current amount of this bet that was lapsed
+    size_cancelled: Optional[Size] = None  # Current amount of this bet that was cancelled
+    size_voided: Optional[Size] = None  # Current amount of this bet that was voided
+    customer_order_ref: Optional[CustomerOrderRef] = None  # Customer Order Reference
+    customer_strategy_ref: Optional[CustomerStrategyRef] = None  # Customer Strategy Reference
 
 
 class Match(BaseMessage, kw_only=True, frozen=True):
-    """An individual bet Match, or rollup by price or avg price. Rollup depends on
-    the requested MatchProjection.
+    """An individual bet Match, or rollup by price or avg price.
+
+    Rollup depends on the requested MatchProjection.
     """
 
-    betId: Optional[BetId] = None  # Bet ID (present if no rollup)
-    matchId: Optional[MatchId] = None  # Match ID (present if no rollup)
+    bet_id: Optional[BetId] = None  # Bet ID (present if no rollup)
+    match_id: Optional[MatchId] = None  # Match ID (present if no rollup)
     side: Side  # Side (BACK or LAY)
     price: Price  # Match price
     size: Size  # Size matched at
-    matchDate: Optional[Date] = None  # Match date (present if no rollup)
+    match_date: Optional[Date] = None  # Match date (present if no rollup)
 
 
 class MarketVersion(BaseMessage, frozen=True):
     version: Optional[int] = None  # A non-monotonically increasing number indicating market changes
 
 
 class MarketRates(BaseMessage, frozen=True):
-    marketBaseRate: float  # Market base rate
-    discountAllowed: bool  # Indicates whether discount is allowed on this market
+    market_base_rate: float  # Market base rate
+    discount_allowed: bool  # Indicates whether discount is allowed on this market
 
 
 class MarketLicence(BaseMessage, frozen=True):
     wallet: str  # Wallet from which funds will be taken when betting on this market
     rules: Optional[str] = None
-    rulesHasDate: Optional[bool] = None  # Indicates whether the market's start date and time are relevant to the rules
+    rules_has_date: Optional[bool] = None  # Markets start date and time are relevant to the rules
     clarifications: Optional[str] = None  # Clarifications to the rules for the market
 
 
 class MarketDescription(BaseMessage, kw_only=True, frozen=True):
-    persistenceEnabled: bool  # Indicates if the market supports 'Keep' bets if turned in-play
-    bspMarket: bool  # Indicates if the market supports Betfair SP betting
-    marketTime: Date  # Scheduled start time of the market
-    suspendTime: Date  # Next time the market will be suspended for betting, usually just marketTime
-    settleTime: Optional[Date] = None
-    bettingType: MarketBettingType
-    turnInPlayEnabled: bool  # Indicates if the market is set to turn in-play
-    marketType: str  # Market base type
+    persistence_enabled: bool  # Indicates if the market supports 'Keep' bets if turned in-play
+    bsp_market: bool  # Indicates if the market supports Betfair SP betting
+    market_time: Date  # Scheduled start time of the market
+    suspend_time: Date  # Next time the market will be suspended for betting, usually just marketTime
+    settle_time: Optional[Date] = None
+    betting_type: MarketBettingType
+    turn_in_play_enabled: bool  # Indicates if the market is set to turn in-play
+    market_type: str  # Market base type
     regulator: str  # Market regulator
-    marketBaseRate: float  # Commission rate applicable to the market
-    discountAllowed: bool  # Indicates whether user's discount rate is taken into account on this
+    market_base_rate: float  # Commission rate applicable to the market
+    discount_allowed: bool  # Indicates whether user's discount rate is taken into account on this
     wallet: Optional[str] = None  # The wallet to which the market belongs
     rules: Optional[str] = None  # The wallet to which the market belongs
-    rulesHasDate: Optional[bool] = None  # Indicates whether rules have a date included
-    eachWayDivisor: Optional[float] = None  # Divisor for EACH_WAY market type
+    rules_has_date: Optional[bool] = None  # Indicates whether rules have a date included
+    each_way_divisor: Optional[float] = None  # Divisor for EACH_WAY market type
     clarifications: Optional[str] = None  # Additional information regarding the market
-    lineRangeInfo: Optional[MarketLineRangeInfo] = None  # Line range info for line markets
-    raceType: Optional[str] = None  # External identifier of a race type
-    priceLadderDescription: Optional[PriceLadderDescription] = None  # Details about the price ladder in use
+    line_range_info: Optional[MarketLineRangeInfo] = None  # Line range info for line markets
+    race_type: Optional[str] = None  # External identifier of a race type
+    price_ladder_description: Optional[PriceLadderDescription] = None  # Details about the price ladder in use
 
 
 class RunnerCatalog(BaseMessage, frozen=True):
     """Information about the Runners (selections) in a market"""
 
-    selectionId: int  # The unique id for the selection
-    runnerName: str  # The name of the runner
+    selection_id: int  # The unique id for the selection
+    runner_name: str  # The name of the runner
 
     # The handicap applies to market with the MarketBettingType ASIAN_HANDICAP_SINGLE_LINE
     # & ASIAN_HANDICAP_DOUBLE_LINE only
     handicap: float
-    sortPriority: Optional[int] = None  # This is marked as REQUIRED in the API doc, but omitted sometimes
+    sort_priority: Optional[int] = None  # This is marked as REQUIRED in the API doc, but omitted sometimes
     metadata: Optional[dict[str, Optional[str]]] = None  # Metadata associated with the runner
 
     @property
-    def runner_name(self):
-        # TODO: This should be gone, as soon all fields are renamed
-        return self.runnerName
-
-    @property
     def runner_id(self):
         # TODO: Careful, selectionId is simply a number for a certain string. It's not
         #       uniquely identifying a team or a certain horse.
-        if self.selectionId:
-            return self.selectionId
-        elif self.metadata.get("runnerId"):
-            return int(self.metadata.get("runnerId"))
+        if self.selection_id:
+            return self.selection_id
+        elif self.metadata.get("runner_id"):
+            return int(self.metadata.get("runner_id"))
         return None
 
 
 class Runner(BaseMessage, frozen=True):
     """The dynamic data about runners in a market"""
 
-    selectionId: int  # The unique id of the runner (selection)
+    selection_id: int  # The unique id of the runner (selection)
     handicap: float  # The handicap
     status: RunnerStatus  # The status of the selection
-    adjustmentFactor: Optional[float] = None  # The adjustment factor applied if the selection is removed
-    lastPriceTraded: Optional[float] = None  # The price of the most recent bet matched on this selection
-    totalMatched: Optional[float] = None  # The total amount matched on this runner
-    removalDate: Optional[Date] = None  # If date and time the runner was removed
+    adjustment_factor: Optional[float] = None  # The adjustment factor applied if the selection is removed
+    last_price_traded: Optional[float] = None  # The price of the most recent bet matched on this selection
+    total_matched: Optional[float] = None  # The total amount matched on this runner
+    removal_date: Optional[Date] = None  # If date and time the runner was removed
     sp: Optional[StartingPrices] = None  # The BSP related prices for this runner
     ex: Optional[ExchangePrices] = None  # The Exchange prices available for this runner
     orders: Optional[list[Order]] = None  # List of orders in the market
     matches: Optional[list[Match]] = None  # List of matches (i.e., orders that have been fully or partially executed)
-    matchesByStrategy: Optional[dict[str, Match]] = None  # List of matches for each strategy, ordered by matched data
+    matches_by_strategy: Optional[dict[str, Match]] = None  # List of matches for each strategy, ordered by matched data
 
 
 class MarketCatalogue(BaseMessage, frozen=True):
-    marketId: MarketId  # The unique identifier for the market
-    marketName: str  # The name of the market
-    marketStartTime: Optional[Date] = None  # Only returned when the MARKET_START_TIME enum is requested
+    market_id: MarketId  # The unique identifier for the market
+    market_name: str  # The name of the market
+    market_start_time: Optional[Date] = None  # Only returned when the MARKET_START_TIME enum is requested
     description: Optional[MarketDescription] = None  # Details about the market
-    totalMatched: Optional[float] = None  # The total amount of money matched on the market
+    total_matched: Optional[float] = None  # The total amount of money matched on the market
     runners: Optional[list[RunnerCatalog]] = None  # The runners (selections) contained in the market
-    eventType: Optional[EventType] = None  # The Event Type the market is contained within
+    event_type: Optional[EventType] = None  # The Event Type the market is contained within
     competition: Optional[Competition] = None  # The competition the market is contained within
     event: Optional[Event] = None  # The event the market is contained within
 
 
 class KeyLineSelection(BaseMessage, frozen=True):
     """Description of a market's key line selection"""
 
-    selectionId: SelectionId  # Selection ID of the runner in the key line handicap
+    selection_id: SelectionId  # Selection ID of the runner in the key line handicap
     handicap: Handicap  # Handicap value of the key line
 
 
 class KeyLineDescription(BaseMessage, frozen=True):
     """A list of KeyLineSelection objects describing the key line for the market"""
 
-    keyLine: list[KeyLineSelection]  # A list of KeyLineSelection objects
+    key_line: list[KeyLineSelection]  # A list of KeyLineSelection objects
 
 
 class MarketBook(BaseMessage, frozen=True):
     """The dynamic data in a market"""
 
-    marketId: MarketId  # The unique identifier for the market
-    isMarketDataDelayed: bool  # True if the data returned by listMarketBook will be delayed
+    market_id: MarketId  # The unique identifier for the market
+    is_market_data_delayed: bool  # True if the data returned by listMarketBook will be delayed
     status: Optional[MarketStatus] = None  # The status of the market
-    betDelay: Optional[int] = None  # The number of seconds an order is held until it is submitted into the market
-    bspReconciled: Optional[bool] = None  # True if the market starting price has been reconciled
+    bet_delay: Optional[int] = None  # The number of seconds an order is held until it is submitted into the market
+    bsp_reconciled: Optional[bool] = None  # True if the market starting price has been reconciled
     complete: Optional[bool] = None  # If false, runners may be added to the market
     inplay: Optional[bool] = None  # True if the market is currently in play
-    numberOfWinners: Optional[int] = None  # The number of selections that could be settled as winners
-    numberOfRunners: Optional[int] = None  # The number of runners in the market
-    numberOfActiveRunners: Optional[int] = None  # The number of runners that are currently active
-    lastMatchTime: Optional[Date] = None  # The most recent time an order was executed
-    totalMatched: Optional[float] = None  # The total amount matched on the market
-    totalAvailable: Optional[float] = None  # The total amount of orders that remain unmatched
-    crossMatching: Optional[bool] = None  # True if cross matching is enabled for this market
-    runnersVoidable: Optional[bool] = None  # True if runners in the market can be voided
+    number_of_winners: Optional[int] = None  # The number of selections that could be settled as winners
+    number_of_runners: Optional[int] = None  # The number of runners in the market
+    number_of_active_runners: Optional[int] = None  # The number of runners that are currently active
+    last_match_time: Optional[Date] = None  # The most recent time an order was executed
+    total_matched: Optional[float] = None  # The total amount matched on the market
+    total_available: Optional[float] = None  # The total amount of orders that remain unmatched
+    cross_matching: Optional[bool] = None  # True if cross matching is enabled for this market
+    runners_voidable: Optional[bool] = None  # True if runners in the market can be voided
     version: Optional[int] = None  # The version of the market
     runners: Optional[list[Runner]] = None  # Information about the runners (selections) in the market
-    keyLineDescription: Optional[KeyLineDescription] = None  # Description of a market's key line
+    key_line_description: Optional[KeyLineDescription] = None  # Description of a market's key line
 
 
 class ItemDescription(BaseMessage, frozen=True):
     """
     This object contains some text which may be useful to render a betting history view.
     It offers no long-term warranty as to the correctness of the text.
     """
 
-    eventTypeDesc: Optional[str] = None  # The event type name translated into the requested locale
-    eventDesc: Optional[str] = None  # The event name or openDate + venue translated into the requested locale
-    marketDesc: Optional[str] = None  # The market name or racing market type translated into the requested locale
-    marketType: Optional[str] = None  # The market type e.g. MATCH_ODDS, PLACE, WIN etc.
-    marketStartTime: Optional[Date] = None  # The start time of the market in ISO-8601 format, not translated
-    runnerDesc: Optional[str] = None  # The runner name translated into the requested locale
-    numberOfWinners: Optional[int] = None  # The number of winners on a market
-    eachWayDivisor: Optional[float] = None  # The divisor for the EACH_WAY market type
+    event_type_desc: Optional[str] = None  # The event type name translated into the requested locale
+    event_desc: Optional[str] = None  # The event name or openDate + venue translated into the requested locale
+    market_desc: Optional[str] = None  # The market name or racing market type translated into the requested locale
+    market_type: Optional[str] = None  # The market type e.g. MATCH_ODDS, PLACE, WIN etc.
+    market_start_time: Optional[Date] = None  # The start time of the market in ISO-8601 format, not translated
+    runner_desc: Optional[str] = None  # The runner name translated into the requested locale
+    number_of_winners: Optional[int] = None  # The number of winners on a market
+    each_way_divisor: Optional[float] = None  # The divisor for the EACH_WAY market type
 
 
 class ClearedOrderSummary(BaseMessage, frozen=True):
     """Summary of a cleared order"""
 
-    eventTypeId: Optional[EventTypeId] = None  # The id of the event type bet on
-    eventId: Optional[EventId] = None  # The id of the event bet on
-    marketId: Optional[MarketId] = None  # The id of the market bet on
-    selectionId: Optional[int] = None  # The id of the selection bet on
+    event_type_id: Optional[EventTypeId] = None  # The id of the event type bet on
+    event_id: Optional[EventId] = None  # The id of the event bet on
+    market_id: Optional[MarketId] = None  # The id of the market bet on
+    selection_id: Optional[int] = None  # The id of the selection bet on
     handicap: Optional[float] = None  # The handicap value for Asian handicap markets
-    betId: Optional[BetId] = None  # The id of the bet
-    placedDate: Optional[Date] = None  # The date the bet order was placed by the customer
-    persistenceType: Optional[PersistenceType] = None  # The turn in play persistence state of the order
-    orderType: Optional[OrderType] = None
+    bet_id: Optional[BetId] = None  # The id of the bet
+    placed_date: Optional[Date] = None  # The date the bet order was placed by the customer
+    persistence_type: Optional[PersistenceType] = None  # The turn in play persistence state of the order
+    order_type: Optional[OrderType] = None
     side: Optional[Side] = None  # Whether the bet was a back or lay bet
-    itemDescription: Optional[ItemDescription] = None  # Container for ancillary data and localized text
-    betOutcome: Optional[str] = None  # The settlement outcome of the bet
-    priceRequested: Optional[Price] = None  # The average requested price across all settled bet orders under this item
-    settledDate: Optional[Date] = None  # The date and time the bet order was settled by Betfair
-    lastMatchedDate: Optional[Date] = None  # The date and time the last bet order was matched by Betfair
-    betCount: Optional[int] = None  # The number of actual bets within this grouping
+    item_description: Optional[ItemDescription] = None  # Container for ancillary data and localized text
+    bet_outcome: Optional[str] = None  # The settlement outcome of the bet
+    price_requested: Optional[Price] = None  # The average requested price across all settled bet orders under this item
+    settled_date: Optional[Date] = None  # The date and time the bet order was settled by Betfair
+    last_matched_date: Optional[Date] = None  # The date and time the last bet order was matched by Betfair
+    bet_count: Optional[int] = None  # The number of actual bets within this grouping
 
     # The cumulative amount of commission paid by the customer across all bets under this item
     commission: Optional[Size] = None
-    priceMatched: Optional[Price] = None  # The average matched price across all settled bets or bet fragments
-    priceReduced: Optional[bool] = None  # Indicates if the matched price was affected by a reduction factor
-    sizeSettled: Optional[Size] = None  # The cumulative bet size that was settled as matched or voided under this item
+    price_matched: Optional[Price] = None  # The average matched price across all settled bets or bet fragments
+    price_reduced: Optional[bool] = None  # Indicates if the matched price was affected by a reduction factor
+    size_settled: Optional[Size] = None  # The cumulative bet size that was settled as matched or voided under this item
     profit: Optional[Size] = None  # The profit or loss gained on this line
-    sizeCancelled: Optional[Size] = None  # The amount of the bet that was cancelled
-    customerOrderRef: Optional[CustomerOrderRef] = None  # The order reference defined by the customer for the bet order
-    customerStrategyRef: Optional[
-        CustomerStrategyRef
-    ] = None  # The strategy reference defined by the customer for the bet order
+    size_cancelled: Optional[Size] = None  # The amount of the bet that was cancelled
+    customer_order_ref: Optional[CustomerOrderRef] = None  # Defined by the customer for the bet order
+    customer_strategy_ref: Optional[CustomerStrategyRef] = None  # Defined by the customer for the bet order
 
 
 class ClearedOrderSummaryReport(BaseMessage, frozen=True):
     """A container representing search results"""
 
-    clearedOrders: list[ClearedOrderSummary]  # The list of cleared orders returned by the query
-    moreAvailable: bool  # Indicates whether there are further result items beyond this page
+    cleared_orders: list[ClearedOrderSummary]  # The list of cleared orders returned by the query
+    more_available: bool  # Indicates whether there are further result items beyond this page
 
 
 class RunnerId(BaseMessage, frozen=True):
     """Unique identifier for a runner"""
 
-    marketId: MarketId  # The id of the market bet on
-    selectionId: int  # The id of the selection bet on
+    market_id: MarketId  # The id of the market bet on
+    selection_id: int  # The id of the selection bet on
     handicap: Optional[float] = None  # The handicap associated with the runner in case of Asian handicap markets
 
 
 class CurrentItemDescription(BaseMessage, frozen=True):
     """This object contains ancillary information about the item"""
 
-    marketVersion: MarketVersion  # The relevant version of the market for this item
+    market_version: MarketVersion  # The relevant version of the market for this item
 
 
 class CurrentOrderSummary(BaseMessage, frozen=True):
     """Summary of a current order"""
 
-    betId: BetId  # The bet ID of the original place order
-    marketId: MarketId  # The market ID the order is for
-    selectionId: int  # The selection ID the order is for
+    bet_id: BetId  # The bet ID of the original place order
+    market_id: MarketId  # The market ID the order is for
+    selection_id: int  # The selection ID the order is for
     handicap: float  # The handicap associated with the runner in case of Asian handicap markets
-    priceSize: PriceSize  # The price and size of the bet
-    bspLiability: Size  # The liability of a given BSP bet
+    price_size: PriceSize  # The price and size of the bet
+    bsp_liability: Size  # The liability of a given BSP bet
     side: Side  # BACK/LAY
     status: OrderStatus  # The status of the order
-    persistenceType: PersistenceType  # What to do with the order at turn-in-play
-    orderType: OrderType  # BSP Order type
-    placedDate: Date  # The date the bet was placed
-    matchedDate: Date  # The date of the last matched bet fragment
-    averagePriceMatched: Optional[Price] = None  # The average price matched at
-    sizeMatched: Optional[Size] = None
-    sizeRemaining: Optional[Size] = None
-    sizeLapsed: Optional[Size] = None
-    sizeCancelled: Optional[Size] = None
-    sizeVoided: Optional[Size] = None
-    regulatorAuthCode: Optional[str] = None
-    regulatorCode: Optional[str] = None
-    customerOrderRef: Optional[str] = None  # The order reference defined by the customer for this bet
-    customerStrategyRef: Optional[str] = None  # The strategy reference defined by the customer for this bet
-    currentItemDescription: Optional[CurrentItemDescription] = None  # Container for ancillary data for this item
+    persistence_type: PersistenceType  # What to do with the order at turn-in-play
+    order_type: OrderType  # BSP Order type
+    placed_date: Date  # The date the bet was placed
+    matched_date: Date  # The date of the last matched bet fragment
+    average_price_matched: Optional[Price] = None  # The average price matched at
+    size_matched: Optional[Size] = None
+    size_remaining: Optional[Size] = None
+    size_lapsed: Optional[Size] = None
+    size_cancelled: Optional[Size] = None
+    size_voided: Optional[Size] = None
+    regulator_auth_code: Optional[str] = None
+    regulator_code: Optional[str] = None
+    customer_order_ref: Optional[str] = None  # The order reference defined by the customer for this bet
+    customer_strategy_ref: Optional[str] = None  # The strategy reference defined by the customer for this bet
+    current_item_description: Optional[CurrentItemDescription] = None  # Container for ancillary data for this item
 
 
 class CurrentOrderSummaryReport(BaseMessage, frozen=True):
     """A container representing search results"""
 
-    currentOrders: list[CurrentOrderSummary]  # The list of current orders returned by the query
-    moreAvailable: bool  # Indicates whether there are further result items beyond this page
+    current_orders: list[CurrentOrderSummary]  # The list of current orders returned by the query
+    more_available: bool  # Indicates whether there are further result items beyond this page
 
 
 class LimitOrder(BaseMessage, frozen=True):
     """Place a new LIMIT order (simple exchange bet for immediate execution)"""
 
     size: Size
     price: Price
-    persistenceType: PersistenceType
-    timeInForce: Optional[TimeInForce] = None
-    minFillSize: Optional[Size] = None
-    betTargetType: Optional[BetTargetType] = None
-    betTargetSize: Optional[Size] = None
+    persistence_type: PersistenceType
+    time_in_force: Optional[TimeInForce] = None
+    min_fill_size: Optional[Size] = None
+    bet_target_type: Optional[BetTargetType] = None
+    bet_target_size: Optional[Size] = None
 
 
 class LimitOnCloseOrder(BaseMessage, frozen=True):
     liability: Size
     price: Price
 
 
 class MarketOnCloseOrder(BaseMessage, frozen=True):
     liability: Size
 
 
 class PlaceInstruction(BaseMessage, kw_only=True, frozen=True):
     """Instruction to place a new order"""
 
-    orderType: OrderType  # The order type
-    selectionId: SelectionId  # The selection ID
+    order_type: OrderType  # The order type
+    selection_id: SelectionId  # The selection ID
     handicap: Optional[Handicap] = None  # The handicap associated with the runner in case of Asian handicap markets
     side: Side  # Back or Lay
-    limitOrder: Optional[LimitOrder] = None  # A simple exchange bet for immediate execution
+    limit_order: Optional[LimitOrder] = None  # A simple exchange bet for immediate execution
 
     # Bets matched if the returned starting price is better than a specified price
-    limitOnCloseOrder: Optional[LimitOnCloseOrder] = None
+    limit_on_close_order: Optional[LimitOnCloseOrder] = None
 
     # Bets matched and settled at a price representative of the market at the point it turns in-play
-    marketOnCloseOrder: Optional[MarketOnCloseOrder] = None
-    customerOrderRef: Optional[str] = None  # An optional reference to identify instructions
+    market_on_close_order: Optional[MarketOnCloseOrder] = None
+    customer_order_ref: Optional[str] = None  # An optional reference to identify instructions
 
 
 class PlaceInstructionReport(BaseMessage, kw_only=True, frozen=True):
     """Report for a place instruction"""
 
     status: InstructionReportStatus  # The instruction report status
-    errorCode: Optional[InstructionReportErrorCode] = None
-    orderStatus: Optional[OrderStatus] = None
+    error_code: Optional[InstructionReportErrorCode] = None
+    order_status: Optional[OrderStatus] = None
     instruction: PlaceInstruction  # The place instruction
-    betId: Optional[BetId] = None  # The bet ID of the placed order, if successful
-    placedDate: Optional[Date] = None  # The date and time the bet was placed, if successful
-    averagePriceMatched: Optional[Price] = None  # The average price matched at, if successful
-    sizeMatched: Optional[Size] = None  # The current amount of the bet that was matched, if successful
+    bet_id: Optional[BetId] = None  # The bet ID of the placed order, if successful
+    placed_date: Optional[Date] = None  # The date and time the bet was placed, if successful
+    average_price_matched: Optional[Price] = None  # The average price matched at, if successful
+    size_matched: Optional[Size] = None  # The current amount of the bet that was matched, if successful
 
 
 class PlaceExecutionReport(BaseMessage, kw_only=True, frozen=True):
-    customerRef: Optional[CustomerRef] = None  # Echo of the customer reference if passed
+    customer_ref: Optional[CustomerRef] = None  # Echo of the customer reference if passed
     status: ExecutionReportStatus  # The execution report status
-    errorCode: Optional[ExecutionReportErrorCode] = None  # The execution report error code
-    marketId: Optional[MarketId] = None  # Echo of the market ID passed
-    instructionReports: Optional[list[PlaceInstructionReport]] = None  # The list of place instruction reports
+    error_code: Optional[ExecutionReportErrorCode] = None  # The execution report error code
+    market_id: Optional[MarketId] = None  # Echo of the market ID passed
+    instruction_reports: Optional[list[PlaceInstructionReport]] = None  # The list of place instruction reports
 
 
 class CancelInstruction(BaseMessage, frozen=True):
     """Instruction to fully or partially cancel an order (only applies to LIMIT orders)"""
 
-    betId: BetId
+    bet_id: BetId
     # If supplied then this is a partial cancel. Should be set to 'null' if no size
     # reduction is required.
-    sizeReduction: Optional[Size] = None
+    size_reduction: Optional[Size] = None
 
 
 class ReplaceInstruction(BaseMessage, frozen=True):
     """Instruction to replace a LIMIT or LIMIT_ON_CLOSE order at a new price."""
 
-    betId: BetId  # Unique identifier for the bet
-    newPrice: Price  # The price to replace the bet at
+    bet_id: BetId  # Unique identifier for the bet
+    new_price: Price  # The price to replace the bet at
 
 
 class CancelInstructionReport(BaseMessage, kw_only=True, frozen=True):
     status: InstructionReportStatus  # Whether the command succeeded or failed
-    errorCode: Optional[InstructionReportErrorCode] = None  # Cause of failure, or null if command succeeds
+    error_code: Optional[InstructionReportErrorCode] = None  # Cause of failure, or null if command succeeds
     instruction: Optional[CancelInstruction] = None  # The instruction that was requested
-    sizeCancelled: Optional[float] = None  # The API states, that this is mandatory, but it's skipped in case of error
-    cancelledDate: Optional[Date] = None
+    size_cancelled: Optional[float] = None  # The API states, that this is mandatory, but it's skipped in case of error
+    cancelled_date: Optional[Date] = None
 
 
 class CancelExecutionReport(BaseMessage, kw_only=True, frozen=True):
-    customerRef: Optional[CustomerRef] = None  # Echo of the customerRef if passed
+    customer_ref: Optional[CustomerRef] = None  # Echo of the customerRef if passed
     status: ExecutionReportStatus
-    errorCode: Optional[ExecutionReportErrorCode] = None
-    marketId: Optional[MarketId] = None  # Echo of marketId passed
-    instructionReports: Optional[list[CancelInstructionReport]] = None
+    error_code: Optional[ExecutionReportErrorCode] = None
+    market_id: Optional[MarketId] = None  # Echo of marketId passed
+    instruction_reports: Optional[list[CancelInstructionReport]] = None
 
 
 class ReplaceInstructionReport(BaseMessage, frozen=True):
     status: InstructionReportStatus  # Whether the command succeeded or failed
-    errorCode: Optional[InstructionReportErrorCode] = None  # Cause of failure, or null if command succeeds
-    cancelInstructionReport: Optional[CancelInstructionReport] = None  # Cancellation report for the original order
-    placeInstructionReport: Optional[PlaceInstructionReport] = None  # Placement report for the new order
+    error_code: Optional[InstructionReportErrorCode] = None  # Cause of failure, or null if command succeeds
+    cancel_instruction_report: Optional[CancelInstructionReport] = None  # Cancellation report for the original order
+    place_instruction_report: Optional[PlaceInstructionReport] = None  # Placement report for the new order
 
 
 class ReplaceExecutionReport(BaseMessage, kw_only=True, frozen=True):
-    customerRef: Optional[CustomerRef] = None  # Echo of the customerRef if passed.
+    customer_ref: Optional[CustomerRef] = None  # Echo of the customerRef if passed.
     status: ExecutionReportStatus
-    errorCode: Optional[ExecutionReportErrorCode] = None
-    marketId: Optional[MarketId] = None  # Echo of marketId passed
-    instructionReports: Optional[list[ReplaceInstructionReport]] = None
+    error_code: Optional[ExecutionReportErrorCode] = None
+    market_id: Optional[MarketId] = None  # Echo of marketId passed
+    instruction_reports: Optional[list[ReplaceInstructionReport]] = None
 
 
 class UpdateInstruction(BaseMessage, frozen=True):
     """Instruction to update LIMIT bet's persistence of an order that do not affect exposure"""
 
-    betId: BetId  # Unique identifier for the bet
-    newPersistenceType: PersistenceType  # The new persistence type to update this bet to
+    bet_id: BetId  # Unique identifier for the bet
+    new_persistence_type: PersistenceType  # The new persistence type to update this bet to
 
 
 class UpdateInstructionReport(BaseMessage, kw_only=True, frozen=True):
     status: InstructionReportStatus  # Whether the command succeeded or failed
-    errorCode: Optional[InstructionReportErrorCode] = None  # Cause of failure, or null if command succeeds
+    error_code: Optional[InstructionReportErrorCode] = None  # Cause of failure, or null if command succeeds
     instruction: UpdateInstruction  # The instruction that was requested
 
 
 class UpdateExecutionReport(BaseMessage, frozen=True):
-    customerRef: Optional[CustomerRef]  # Echo of the customerRef if passed.
+    customer_ref: Optional[CustomerRef]  # Echo of the customerRef if passed.
     status: ExecutionReportStatus
-    errorCode: Optional[ExecutionReportErrorCode]
-    marketId: Optional[MarketId]  # Echo of marketId passed
-    instructionReports: Optional[list[UpdateInstructionReport]]
+    error_code: Optional[ExecutionReportErrorCode]
+    market_id: Optional[MarketId]  # Echo of marketId passed
+    instruction_reports: Optional[list[UpdateInstructionReport]]
 
 
 class ExBestOffersOverrides(BaseMessage, frozen=True):
     """Options to alter the default representation of best offer prices"""
 
-    bestPricesDepth: Optional[int] = None  # The maximum number of prices to return on each side for each runner
-    rollupModel: Optional[RollupModel] = None  # The model to use when rolling up available sizes
-    rollupLimit: Optional[int] = None  # The volume limit to use when rolling up returned sizes
-    rollupLiabilityThreshold: Optional[float] = None  # Only applicable when rollupModel is MANAGED_LIABILITY
-    rollupLiabilityFactor: Optional[int] = None  # Only applicable when rollupModel is MANAGED_LIABILITY
+    best_prices_depth: Optional[int] = None  # The maximum number of prices to return on each side for each runner
+    rollup_model: Optional[RollupModel] = None  # The model to use when rolling up available sizes
+    rollup_limit: Optional[int] = None  # The volume limit to use when rolling up returned sizes
+    rollup_liability_threshold: Optional[float] = None  # Only applicable when rollupModel is MANAGED_LIABILITY
+    rollup_liability_factor: Optional[int] = None  # Only applicable when rollupModel is MANAGED_LIABILITY
 
 
 class PriceProjection(BaseMessage, frozen=True):
     """Selection criteria of the returning price data"""
 
-    priceData: Optional[set[PriceData]] = None  # The basic price data you want to receive in the response
+    price_data: Optional[set[PriceData]] = None  # The basic price data you want to receive in the response
 
     # Options to alter the default representation of best offer prices
-    exBestOffersOverrides: Optional[ExBestOffersOverrides] = None
+    ex_best_offers_overrides: Optional[ExBestOffersOverrides] = None
     virtualise: Optional[bool] = None  # Indicates if the returned prices should include virtual prices
 
     # Indicates if the volume returned at each price point should be the absolute value or a
     # cumulative sum of volumes available at the price and all better prices. If unspecified
     # defaults to false. Applicable to EX_BEST_OFFERS and EX_ALL_OFFERS price projections.
     # Not supported as yet.
-    rolloverStakes: Optional[bool] = None
+    rollover_stakes: Optional[bool] = None
 
 
 class RunnerProfitAndLoss(BaseMessage, frozen=True):
     """Profit and loss if selection wins or loses"""
 
-    selectionId: Optional[SelectionId] = None  # The unique identifier for the selection
-    ifWin: Optional[float] = None  # Profit or loss for the market if this selection is the winner
-    ifLose: Optional[float] = None  # Profit or loss for the market if this selection is the loser
+    selection_id: Optional[SelectionId] = None  # The unique identifier for the selection
+    if_win: Optional[float] = None  # Profit or loss for the market if this selection is the winner
+    if_lose: Optional[float] = None  # Profit or loss for the market if this selection is the loser
 
     # Profit or loss for the market if this selection is placed (applies to marketType EACH_WAY only)
-    ifPlace: Optional[float] = None
+    if_place: Optional[float] = None
 
 
 class MarketProfitAndLoss(BaseMessage, frozen=True):
     """Profit and loss in a market"""
 
-    marketId: Optional[MarketId] = None  # The unique identifier for the market
-    commissionApplied: Optional[float] = None  # The commission rate applied to P&L values
-    profitAndLosses: Optional[list[RunnerProfitAndLoss]] = None  # Calculated profit and loss data
+    market_id: Optional[MarketId] = None  # The unique identifier for the market
+    commission_applied: Optional[float] = None  # The commission rate applied to P&L values
+    profit_and_losses: Optional[list[RunnerProfitAndLoss]] = None  # Calculated profit and loss data
```

### Comparing `betfair_parser-0.2.2/betfair_parser/spec/common.py` & `betfair_parser-0.2.3/betfair_parser/spec/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     return msgspec.json.decode(raw, type=type, dec_hook=decode_intfloat)
 
 
 def encode(data):
     return msgspec.json.encode(data, enc_hook=encode_intfloat)
 
 
-class BaseMessage(msgspec.Struct, kw_only=True, forbid_unknown_fields=True, frozen=True):
+class BaseMessage(msgspec.Struct, kw_only=True, forbid_unknown_fields=True, frozen=True, rename="camel"):
     def validate(self):
         return bool(decode(encode(self), type=type(self)))
 
     def to_dict(self):
         return msgspec.structs.asdict(self)
 
 
@@ -83,25 +83,30 @@
 
 
 class ErrorResponse(RPC, kw_only=True, frozen=True):
     error: JsonError
 
 
 class APIException(BaseMessage, Generic[ErrorCode], kw_only=True, frozen=True):
-    errorCode: ErrorCode
-    errorDetails: Optional[str] = None  # The stack trace of the error
-    requestUUID: Optional[str] = None
+    error_code: ErrorCode
+    error_details: Optional[str] = None  # The stack trace of the error
+    request_uuid: Optional[str] = msgspec.field(name="requestUUID", default=None)
 
 
 class Request(RPC, kw_only=True, frozen=True):
     method: str
     params: msgspec.Struct
     response_type = None  # not to be serialized, so no type definition
     throws = APIException[APIExceptionCode]  # not to be serialized, so no type definition
 
+    @classmethod
+    def with_params(cls, **kwargs):
+        params_cls = cls.__annotations__["params"]
+        return cls(params=params_cls(**kwargs))
+
 
 # Type aliases with minimalistic validation
 
 Date = Annotated[datetime.datetime, msgspec.Meta(title="Date", tz=True)]
 SelectionId = Annotated[IntStr, msgspec.Meta(title="SelectionId")]
 Venue = Annotated[str, msgspec.Meta(title="Venue")]
 MarketId = Annotated[str, msgspec.Meta(title="MarketId")]
```

### Comparing `betfair_parser-0.2.2/betfair_parser/spec/error.py` & `betfair_parser-0.2.3/betfair_parser/spec/error.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.2/betfair_parser/spec/heartbeat.py` & `betfair_parser-0.2.3/betfair_parser/spec/heartbeat.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,27 +10,27 @@
     CANCELLATION_REQUEST_ERROR = doc("There was an error requesting cancellation, no bets have been cancelled")
     CANCELLATION_STATUS_UNKNOWN = doc("There was no response from requesting cancellation, cancellation status unknown")
 
 
 class HeartbeatReport(BaseMessage, frozen=True):
     """Response from heartbeat operation."""
 
-    actionPerformed: ActionPerformed  # The action performed since your last heartbeat request.
-    actualTimeoutSeconds: int  # The actual timeout applied to your heartbeat request
+    action_performed: ActionPerformed  # The action performed since your last heartbeat request.
+    actual_timeout_seconds: int  # The actual timeout applied to your heartbeat request
 
 
-class heartbeatParams(BaseMessage, frozen=True):
+class _HeartbeatParams(BaseMessage, frozen=True):
     # Maximum period in seconds that may elapse (without a subsequent heartbeat request),
     # before a cancellation request is automatically submitted on your behalf. The minimum
     # value is 10, the maximum value permitted is 300.
-    preferredTimeoutSeconds: int
+    preferred_timeout_seconds: int
 
 
-class heartbeat(Request, kw_only=True, frozen=True):
+class Heartbeat(Request, kw_only=True, frozen=True):
     """
     Returns a list of Competitions (i.e., World Cup 2013) associated with the markets selected by
     the MarketFilter. Currently only Football markets have an associated competition.
     """
 
     method = "HeartbeatAPING/v1.0/heartbeat"
-    params: heartbeatParams
+    params: _HeartbeatParams
     return_type = Response[HeartbeatReport]
```

### Comparing `betfair_parser-0.2.2/betfair_parser/spec/navigation.py` & `betfair_parser-0.2.3/betfair_parser/spec/navigation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,80 +1,70 @@
 import re
-from enum import Enum
 from typing import ClassVar, Literal, Optional, Union
 
 import msgspec
 
-from betfair_parser.spec.common import BaseMessage, Date, Request
+from betfair_parser.spec.common import BaseMessage, Date, Request, decode, encode
+from betfair_parser.spec.constants import Locale
 
 
 def tag_func(s: str):
     """
     >>> tag_func("EventType")
     'EVENT_TYPE'
 
     >>> tag_func("Group")
     'GROUP'
     """
     return re.sub(r"(?<!^)(?=[A-Z])", "_", s).upper()
 
 
-class Locale(Enum):
-    English = "en"
-    Spanish = "es"
-    Italian = "it"
-    German = "de"
-    Swedish = "sv"
-    Portuguese = "pt"
-    Russian = "ru"
-
-
-class navigationParams(BaseMessage, kw_only=True, frozen=True):
+class _NavigationParams(BaseMessage, kw_only=True, frozen=True):
     locale: Locale
 
 
 class NavigationRequest(Request, kw_only=True, frozen=True):
     """
     Navigation requests - https://docs.developer.betfair.com/display/1smk3cen4v3lu3yomq5qye0ni/Navigation+Data+For+Applications
     """
 
     METHOD_TEMPLATE: ClassVar[str] = "/betting/rest/v1/{locale}/navigation/menu.json"
-    params: navigationParams
+    params: _NavigationParams
     method: str = METHOD_TEMPLATE.format(locale=Locale.English.value)
 
     @classmethod
-    def with_locale(cls, params: navigationParams, locale: Locale):
+    def with_locale(cls, params: _NavigationParams, locale: Locale):
         method = cls.METHOD_TEMPLATE.format(locale=locale.value)
         return msgspec.structs.replace(cls(params=params), method=method)
 
 
 class Market(BaseMessage, tag=tag_func, frozen=True):
     name: str
     id: str
-    exchangeId: str
-    marketType: str
-    marketStartTime: str
-    numberOfWinners: Union[int, str]
+    exchange_id: str
+    market_type: str
+    market_start_time: str
+    number_of_winners: Union[int, str]
 
 
 class Event(BaseMessage, tag=tag_func, frozen=True):
     name: str
     id: str
-    countryCode: str
+    country_code: str
     children: list[Union["Group", "Event", Market]]
 
 
 class Race(BaseMessage, tag=tag_func, frozen=True):
     name: str
     id: str
-    countryCode: str
+    country_code: str
     venue: str
-    startTime: Date
+    start_time: Date
     children: list[Market]
-    raceNumber: Optional[str] = None
+    race_number: Optional[str] = None
 
 
 class Group(BaseMessage, tag=tag_func, frozen=True):
     name: str
     id: str
     children: list[Union["Group", Event]]
 
@@ -90,67 +80,66 @@
 
     type: Literal["GROUP"]
     name: Literal["ROOT"]
     id: int
     children: list[EventType]
 
 
-class FlattenedMarket(BaseMessage, kw_only=True, frozen=True):
+class FlattenedMarket(BaseMessage, kw_only=True, frozen=True, rename=None):
     event_type_name: str
     event_type_id: str
     event_name: Optional[str] = None
     event_id: Optional[str] = None
-    event_countryCode: Optional[str] = None
+    event_country_code: Optional[str] = None
     market_name: str
     market_id: str
-    market_exchangeId: str
-    market_marketType: str
-    market_marketStartTime: str
-    market_numberOfWinners: Union[int, str]
+    market_exchange_id: str
+    market_market_type: str
+    market_market_start_time: str
+    market_number_of_winners: Union[int, str]
     group_name: Optional[str] = None
     group_id: Optional[str] = None
     race_name: Optional[str] = None
     race_id: Optional[str] = None
-    race_countryCode: Optional[str] = None
+    race_country_code: Optional[str] = None
     race_venue: Optional[str] = None
-    race_startTime: Optional[str] = None
-    race_raceNumber: Optional[str] = None
+    race_start_time: Optional[str] = None
+    race_race_number: Optional[str] = None
 
 
 def navigation_to_flatten_markets(navigation: Navigation, **filters) -> list[FlattenedMarket]:
-    flattened = flatten_tree(msgspec.json.decode(msgspec.json.encode(navigation)), **filters)
-    return msgspec.json.decode(msgspec.json.encode(flattened), type=list[FlattenedMarket])
+    flattened = flatten_tree(decode(encode(navigation), type=Navigation), **filters)
+    return decode(encode(flattened), type=list[FlattenedMarket])
 
 
-def flatten_tree(data: dict, **filters):
+def flatten_tree(navigation: dict, **filters):
     """
     Flatten a nested dict into a list of dicts with each nested level combined
     into a single dict.
     """
     results = []
     ignore_keys = ("type", "children")
 
-    def flatten(dict_like, depth: Optional[int] = None):
-        def _filter(k, v):
-            if isinstance(v, str):
-                return k == v
-            elif isinstance(v, (tuple, list)):
-                return k in v
-            else:
-                raise TypeError
+    def _filter(k, v):
+        if isinstance(v, str):
+            return k == v
+        if isinstance(v, (tuple, list)):
+            return k in v
+        raise TypeError
 
+    def flatten(nav_item, depth: Optional[int] = None):
         depth = depth or 0
-        node_type = dict_like["type"].lower()
-        data = {f"{node_type}_{k}": v for k, v in dict_like.items() if k not in ignore_keys}
-        if "children" in dict_like:
-            for child in dict_like["children"]:
+        node_type = tag_func(nav_item.__class__.__name__).lower()
+        data = {f"{node_type}_{k}": v for k, v in nav_item.to_dict().items() if k not in ignore_keys}
+        if hasattr(nav_item, "children"):
+            for child in nav_item.children:
                 for child_data in flatten(child, depth=depth + 1):
                     if depth == 0:
                         if all(_filter(child_data[k], v) for k, v in filters.items()):
                             results.append(child_data)
                     else:
                         yield {**data, **child_data}
         else:
             yield data
 
-    list(flatten(data))
+    list(flatten(navigation))
     return results
```

### Comparing `betfair_parser-0.2.2/betfair_parser/spec/race_status.py` & `betfair_parser-0.2.3/betfair_parser/spec/race_status.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,24 +36,24 @@
     UNEXPECTED_ERROR = doc("An unexpected error occurred retrieving score data")
     LIVE_DATA_TEMPORARILY_UNAVAILABLE = doc(
         "Live Data feed for this event/match is temporarily unavailable, data could potentially be stale"
     )
 
 
 class RaceDetails(BaseMessage, kw_only=True, frozen=True):
-    meetingId: str  # The unique Id for the meeting equivalent to the eventId as returned by listEvents
-    raceId: str  # The unique Id for the race in the format meetingId.raceTime (hhmm)
-    raceStatus: RaceStatus  # The current status of the race.
-    lastUpdated: Date  # This is the time the data was last updated
+    meeting_Id: str  # The unique Id for the meeting equivalent to the eventId as returned by listEvents
+    race_id: str  # The unique Id for the race in the format meetingId.raceTime (hhmm)
+    race_status: RaceStatus  # The current status of the race.
+    last_updated: Date  # This is the time the data was last updated
     sequence: int  # This is the unique identifier associated to each update of the data
-    responseCode: ResponseCode
+    response_code: ResponseCode
 
 
-class listRaceDetailsParams(BaseMessage, frozen=True):
-    meetingIds: Optional[set[str]] = None  # Restricts the results to the specified meeting IDs.
-    raceIds: Optional[set[str]] = None  # Restricts the results to the specified race IDs.
+class _ListRaceDetailsParams(BaseMessage, frozen=True):
+    meeting_ids: Optional[set[str]] = None  # Restricts the results to the specified meeting IDs.
+    race_ids: Optional[set[str]] = None  # Restricts the results to the specified race IDs.
 
 
-class listRaceDetail(Request, kw_only=True, frozen=True):
+class ListRaceDetail(Request, kw_only=True, frozen=True):
     method = "ScoresAPING/v1.0/listRaceDetails"
-    params: listRaceDetailsParams
+    params: _ListRaceDetailsParams
     return_type = Response[list[RaceDetails]]
```

### Comparing `betfair_parser-0.2.2/betfair_parser/spec/streaming/mcm.py` & `betfair_parser-0.2.3/betfair_parser/spec/streaming/mcm.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,31 +18,31 @@
 
 
 class Runner(BaseMessage, frozen=True):
     """
     https://docs.developer.betfair.com/display/1smk3cen4v3lu3yomq5qye0ni/Exchange+Stream+API
     """
 
-    sortPriority: int
+    sort_priority: int
     id: Union[int, str]
     name: Optional[str] = None
     hc: Optional[Union[float, str]] = None
     status: Optional[RunnerStatus] = None
-    adjustmentFactor: Optional[float] = None
-    selectionId: Optional[str] = None
+    adjustment_factor: Optional[float] = None
+    selection_id: Optional[str] = None
     bsp: Optional[Union[str, float]] = None
-    removalDate: Optional[str] = None
+    removal_date: Optional[str] = None
 
     @property
     def handicap(self) -> str:
         return str(self.hc or 0.0)
 
     @property
     def runner_id(self) -> int:
-        return int(self.selectionId or self.id)
+        return int(self.selection_id or self.id)
 
 
 class RunnerKeyLine(BaseMessage, frozen=True):
     id: int
     hc: int
 
 
@@ -51,59 +51,56 @@
 
 
 class MarketDefinition(BaseMessage, kw_only=True, frozen=True):
     """
     https://docs.developer.betfair.com/display/1smk3cen4v3lu3yomq5qye0ni/Exchange+Stream+API
     """
 
-    bspMarket: bool
-    turnInPlayEnabled: bool
-    persistenceEnabled: bool
-    marketBaseRate: Optional[float]
-    marketId: Optional[str] = ""
-    marketName: Optional[str] = ""
-    eventId: str
-    eventTypeId: str
-    numberOfWinners: int
-    bettingType: str
-    marketType: str
-    marketTime: str
-    competitionId: Optional[str] = ""
-    competitionName: Optional[str] = ""
-    eventName: Optional[str] = ""
-    suspendTime: str
-    bspReconciled: bool
+    bsp_market: bool
+    turn_in_play_enabled: bool
+    persistence_enabled: bool
+    market_base_rate: Optional[float]
+    market_id: Optional[str] = ""
+    market_name: Optional[str] = ""
+    event_id: str
+    event_type_id: str
+    number_of_winners: int
+    betting_type: str
+    market_type: str
+    market_time: str
+    competition_id: Optional[str] = ""
+    competition_name: Optional[str] = ""
+    event_name: Optional[str] = ""
+    suspend_time: str
+    bsp_reconciled: bool
     complete: bool
-    inPlay: bool
-    crossMatching: bool
-    runnersVoidable: bool
-    numberOfActiveRunners: int
-    betDelay: int
+    in_play: bool
+    cross_matching: bool
+    runners_voidable: bool
+    number_of_active_runners: int
+    bet_delay: int
     status: MarketStatus
     runners: List[Runner]
     regulators: List[str]
     name: Optional[str] = None
-    openDate: Optional[str] = None
+    open_date: Optional[str] = None
     timezone: Optional[str] = None
     venue: Optional[str] = None
     version: Optional[int] = None
-    countryCode: Optional[str] = None
-    discountAllowed: Optional[bool] = None
-    raceType: Optional[str] = None
-    priceLadderDefinition: Optional[Union[str, PriceLadderDescription]] = None
-    settledTime: Optional[Date] = None
-    keyLineDefinition: Optional[KeyLineDefinition] = None
-    eachWayDivisor: Optional[float] = None
+    country_code: Optional[str] = None
+    discount_allowed: Optional[bool] = None
+    race_type: Optional[str] = None
+    price_ladder_definition: Optional[Union[str, PriceLadderDescription]] = None
+    settled_time: Optional[Date] = None
+    key_line_definition: Optional[KeyLineDefinition] = None
+    each_way_divisor: Optional[float] = None
 
     @property
     def event_type_name(self) -> str:
-        return EVENT_TYPE_TO_NAME[self.eventTypeId]
-
-    def to_dict(self):
-        return {f: getattr(self, f) for f in self.__struct_fields__}
+        return EVENT_TYPE_TO_NAME[self.event_type_id]
 
 
 class AvailableToBack(BaseMessage, array_like=True, frozen=True):
     """AvailableToBack"""
 
     price: float
     volume: float
@@ -193,34 +190,34 @@
 
 class MarketChange(BaseMessage, frozen=True):
     """
     https://docs.developer.betfair.com/display/1smk3cen4v3lu3yomq5qye0ni/Exchange+Stream+API
     """
 
     id: str
-    marketDefinition: Optional[MarketDefinition] = None
+    market_definition: Optional[MarketDefinition] = None
     rc: List[RunnerChange] = []
     img: bool = False
     tv: Optional[float] = None
     con: Optional[bool] = None
 
 
 class MCM(BaseMessage, tag_field="op", tag=str.lower, frozen=True):
     """
     https://docs.developer.betfair.com/display/1smk3cen4v3lu3yomq5qye0ni/Exchange+Stream+API
     """
 
     pt: int
     clk: Optional[str] = None
     id: Optional[int] = None
-    initialClk: Optional[str] = None
-    marketDefinition: Optional[MarketDefinition] = None
+    initial_clk: Optional[str] = None
+    market_definition: Optional[MarketDefinition] = None
     status: Optional[int] = None
-    conflateMs: Optional[int] = None
-    heartbeatMs: Optional[int] = None
+    conflate_ms: Optional[int] = None
+    heartbeat_ms: Optional[int] = None
     ct: Optional[Literal["HEARTBEAT", "SUB_IMAGE", "RESUB_DELTA"]] = None
     mc: List[MarketChange] = []
     con: Optional[bool] = None
 
     @property
     def is_heartbeat(self):
         return self.ct == "HEARTBEAT"
```

### Comparing `betfair_parser-0.2.2/betfair_parser/spec/streaming/ocm.py` & `betfair_parser-0.2.3/betfair_parser/spec/streaming/ocm.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,42 +43,42 @@
 
 class OrderChanges(BaseMessage, frozen=True):
     """
     https://docs.developer.betfair.com/display/1smk3cen4v3lu3yomq5qye0ni/Exchange+Stream+API
     """
 
     id: int
-    fullImage: Optional[bool] = False
+    full_image: Optional[bool] = False
     hc: Optional[float] = None
     uo: Optional[List[UnmatchedOrder]] = []
     mb: Optional[List[MatchedOrder]] = []
     ml: Optional[List[MatchedOrder]] = []
     smc: Optional[dict[str, StrategyMatched]] = None
 
 
 class OrderAccountChange(BaseMessage, frozen=True):
     """
     https://docs.developer.betfair.com/display/1smk3cen4v3lu3yomq5qye0ni/Exchange+Stream+API
     """
 
     id: str
-    accountId: Optional[int] = None
-    fullImage: Optional[bool] = False
+    account_id: Optional[int] = None
+    full_image: Optional[bool] = False
     orc: List[OrderChanges] = []
     closed: Optional[bool] = None
 
 
 class OCM(BaseMessage, tag_field="op", tag=str.lower, frozen=True):
     """
     https://docs.developer.betfair.com/display/1smk3cen4v3lu3yomq5qye0ni/Exchange+Stream+API
     """
 
     id: int
     clk: str
     pt: int
     oc: List[OrderAccountChange] = []
-    initialClk: Optional[str] = None
+    initial_clk: Optional[str] = None
     status: Optional[int] = None
-    conflateMs: Optional[int] = None
-    heartbeatMs: Optional[int] = None
+    conflate_ms: Optional[int] = None
+    heartbeat_ms: Optional[int] = None
     ct: Optional[Literal["HEARTBEAT", "SUB_IMAGE"]] = None
     con: Optional[bool] = None
```

### Comparing `betfair_parser-0.2.2/betfair_parser/spec/streaming/status.py` & `betfair_parser-0.2.3/betfair_parser/spec/streaming/status.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,14 @@
 
     connectionId: str
 
 
 class Status(BaseMessage, tag_field="op", tag=str.lower, frozen=True):
     """Status Message"""
 
-    statusCode: Literal["SUCCESS", "FAILURE"]
-    connectionClosed: bool
+    status_code: Literal["SUCCESS", "FAILURE"]
+    connection_closed: bool
     id: Optional[int] = None
-    connectionsAvailable: Optional[int] = None
-    connectionId: Optional[str] = None
-    errorCode: Optional[StatusErrorCode] = None
-    errorMessage: Optional[str] = None
+    connections_available: Optional[int] = None
+    connection_id: Optional[str] = None
+    error_code: Optional[StatusErrorCode] = None
+    error_message: Optional[str] = None
```

### Comparing `betfair_parser-0.2.2/betfair_parser/strenums.py` & `betfair_parser-0.2.3/betfair_parser/strenums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.2/pyproject.toml` & `betfair_parser-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "betfair_parser"
-version = "0.2.2"
+version = "0.2.3"
 description = ""
 authors = ["Bradley McElroy <bradley.mcelroy@live.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 msgspec = "^0.15.1"
 fsspec = ">=2022"
```

