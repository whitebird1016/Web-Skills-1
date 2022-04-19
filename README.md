# Web-Skills-with-Shikmamaru(1)

<h2>String Skills</h2>
<h3>1 .Compare time</h3>

```
const time1 = "2022-03-02 09:00:00";
const time2 = "2022-03-02 09:00:01";
const overtime = time1 < time2;
// overtime => true
```
<h3>2: Format money</h3>

```
const ThousandNum = num => num.toString().replace(/\B(?=(\d{3})+(?!\d))/g, ",");
const money = ThousandNum(1000000);
// money => '1,000,000'
```
<h3>2: Format money</h3>

```
const ThousandNum = num => num.toString().replace(/\B(?=(\d{3})+(?!\d))/g, ",");
const money = ThousandNum(1000000);
// money => '1,000,000'
```
<h3>3: Generate random ID</h3>

```
const RandomId = len => Math.random().toString(36).substr(3, len);
const id = RandomId(10);
// id => "xdeguewg1f"
```
<h3>4: Generate random HEX color values</h3>

```
const RandomColor = () => "#" + Math.floor(Math.random() * 0xffffff).toString(16).padEnd(6, "0");
const color = RandomColor();
// color => "#2cbf89"
```
<h3>5: Generate star ratings</h3>

```
const StartScore = rate => "★★★★★☆☆☆☆☆".slice(5 - rate, 10 - rate);
const start = StartScore(3);
// start => '★★★☆☆'
```
<h3>6: URL query parameters</h3>

```
const params = new URLSearchParams(location.search.replace(/\?/ig, "")); // location.search = "?name=test&sex=man"
params.has("test"); // true
params.get("sex"); // "man"
```
