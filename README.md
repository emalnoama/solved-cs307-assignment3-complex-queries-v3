Download Link: https://assignmentchef.com/product/solved-cs307-assignment3-complex-queries-v3
<br>
<strong>  </strong>All the questions and the sample result sets in this assignment are using postgres database, and you can import data from <strong>shenzhen_metro.sql</strong>

Your result set, especially the data type and the order of each column, must strictly follow the description and the sample result set in each question.

You need submit “.sql” files for these five questions.

The name of each “.sql” file should be q1, q2, q3, q4, q5 respectively to represent these five questions.

Do not forget to add ‘;’ in the end of each query.

Do not compress them into a folder, please submit them directly.

Please submit those queries into <strong>sakai website</strong> as soon as possible, so that you can get  chance to receive feedback before deadline. After the deadline, we will check the assignment automatically by a script and then given your grade, at that time, any argument about your grade of this assignment will not be accepted.

<strong>Description:                                                                                    </strong>

As a student at the SUSTech, we often use the Shenzhen Metro and buses. In this assignment, we use the data of Shenzhen subway and bus for exercise.

<h1>Problem 1</h1>

<strong>Which stations in Line 1 are not in Line 2, please output the id of those stations in ascending order</strong>

<strong>ᬌ᧗</strong><strong>ڊ</strong><strong>Ӟ</strong><strong>ݩ</strong><strong>ᕚӤጱ</strong><strong>ߺ</strong><strong>Զᒊӧࣁԫ</strong><strong>ݩ</strong><strong>ᕚӤ,᧗</strong><strong>܋</strong><strong>ଧᬌ</strong><strong>ڊ</strong><strong>᫣ᒊidҘ</strong>

<strong>Sample Output:</strong>




<h1>Problem 2</h1>

**The stations on Line 1 distributed in which district? How many stations are there in each district? Please output the district names, the number of stations, and the ranking.

Order of result set is ignored by Testing script

**ӞݩᕚӤጱ᫣ᒊ᮷ߺࣁ૲ړԶ܄ҘᬯԶ܄ྯӻํग़੝ӻંԭ1ݩᕚጱ᫣ᒊҘ᧗ᬌڊᬯԶݷ܄҅᫣ᒊහ ഭ݊զ҅ᰁݷ̶ ၥᦶ෸஺ኼഭଧᳯ᷌

<strong>Sample Output:</strong>

<h1>Problem 3</h1>

<strong>Please output how many subway lines pass through each district and the ranking of the number of subway lines in each district.</strong>

Order of result set is ignored by Testing script. and the null district should not take into consideration.

<strong>ᬌ᧗</strong><strong>ڊ</strong><strong>ྯӻ</strong><strong>܄</strong><strong>ํग़੝ࣈ᱈ᕚ᪠ᕪᬦ҅զ݊ྯӻ</strong><strong>܄</strong><strong>ࣈ᱈ᕚ᪠හᰁጱഭ</strong><strong>ݷ</strong><strong>̶̶</strong>

ၥᦶ෸஺ኼഭଧᳯ᷌, ྦྷਁӾପഝහ܄ҁdistrict҂ԅnullᕑӧᅩᒊጱفᘍᡤ

<strong>Sample Output:</strong>

<h1>Problem 4</h1>

<strong>Please output the subway stations with more than or equal to 10 bus stops around the subway station in each line, </strong><strong>sorted by 1. ascending order of line id, 2. ascending order according to the count of bus stops, 3. descending order of station id. Your result set only return 10 rows from the 16th row</strong>  (You can use limit 10 offset 15)

<strong>ᬌ᧗</strong><strong>ڊ</strong><strong>ྯ๵ᕚ᪠Ӿࣈ᱈ᒊޮᬟ</strong><strong>ل</strong><strong>Իᒊग़ԭ౲ᒵԭ10ጱࣈ᱈᫣ᒊ҅</strong><strong>ଧഭ</strong><strong>ׁ</strong><strong>ഝ 1. line id ጱ</strong><strong>܋</strong><strong>ଧ҅2. </strong><strong>ل</strong><strong>Ի᫣ ጱහᒊ</strong><strong>܋</strong><strong>ଧ҅ 3. station id ጱᴳଧ̶ᬬࢧᕮຎᵞ՗ᒫ16ত୏ᤈ</strong><strong>כ</strong><strong>ኸ10ᤈ</strong>

<strong>Sample Output:</strong>

<h1>Problem 5</h1>

Once upon a time, a new intern comes to Shenzhen metro department to design new stations. As a biology under-graduate, the intern is asked to simply give names to stations instead of designing routes. But the master of department is a strange guy who dislikes the station starts with the same character. For example, if some station starts with ‘Ⴎ’ such like ‘Ⴎԯ’ and another station named ‘Ⴎय़’, then the frequency of this character is 2 (in fact considering all stations, ‘Ⴎ’ presents 7 times).

However, human beings’ ability has the limits and thus the intern cannot find new names with never-used start character. So the master relaxed the limitation and <strong>if the name doesn’t start with the character that shows up the most times, then the name is valid</strong>. However, the limitation asks for <strong>‘the most frequency for each district’</strong>. So, although the character ‘ਪ’ is not valid in Bao’an district, it’s valid in Nanshan district.

Even worse, <strong>some district has the same frequency for some characters</strong>. For example, ‘Ⴎ’, ‘܏’, and ‘ḕ’ are all presents 4 time in Futian district, and all of them are not valid.

The intern has this task daily and nightly in his thought. Finally, on a stellar scintillation night, he had a dream about a short paragraph of SQL code that can list districts, all the most frequency words for each district, and their frequencies. On the next day, as his best friend, you are asked to write this code for him.

<strong>Task: find the most frequency starting characters of stations for each district.</strong> For example, in Nanshan district, you should find all the stations in Nanshan district. And count the first character’s present time, and get the highest frequency characters’ district, character (chr), and present time (cnt).

Hint 1: characters with the same pinyin but not with the same form doesn’t same.

Hint 2: the null district should not take into consideration.

Order of result set is ignored by Testing script

຤ॠ҅ੜA᩸ᒊ᱈ࣈෛԅᨱᨮ҅ԟਫᳪ᮱᱈ࣈࣉႮࣁݷ̶ᆐᘒ҅୮ݷ໏ݶڹਁጱࣈ᱈ᒊਫࣁॡग़ԧ҅ ತᘒکਠقဌአᬦጱݷਁ݈உࢯᵙ҅ੜAݝమ᭿ع୏१ᒫӞӻਁڊሿஉग़ེጱ̶ֺਁݷই҅Ⴎԯ޾Ⴎय़ ᮷զ“Ⴎ”୏१҅ԭฎ҅“Ⴎ”ᚆӧ֢ԅෛݷਁጱ୏१̶

֕Ոᔄጱᚆێฎํຄᴴጱ҅ԭฎੜAᓒ಑ݝ݄ധڊሿ๋ग़ེጱᮎӻ୏१ਁ҅ࣁ୮ڹఘ٭ӥ҅ݝํ“Ⴎ”ӧ ᒧݳᥝ࿢̶֕ฎ҅՜ᬮ಑ᓒ੒ྯӻ܄ತکᧆڊ܄ሿ๋ग़ጱ୏१ਁֺ҅ইਪਞ܄ԅ“ਪ”҅ܖઊ܄ԅ“Ⴎ”̶ᥝ ጱํ҅఺ဳݢ܄ᚆ۱ތग़ӻݶ໏ེහጱਁֺ҅ইᐰኦ܄ጱ“Ⴎ”̵“܏”̵“ḕ”࣐֢ԅࣈ᱈ᒊ୏१ਁڊሿԧࢥ ӧฎ᮷ਁԶᬯᘒེ҅ݳဩጱ̶

ੜAತ᯾໼ॠํԭᕣమज़௏෭کԧӞྦྷSQL᧍ݙ҅๶ଆ՜ತکྯӻڊٖٖ܄ሿ๋ग़ེጱ୏१ਁ̶ᘒ֦ฎ ੜAಓ೘՜ฎԭ҅݋๏ጱঅ๋ڊٟڊٟ֦ᬯྦྷSQL᧍ݙ̶

<strong>ձ</strong><strong>ۓ</strong><strong>ғԅྯӻ</strong><strong>܄</strong><strong>ತ</strong><strong>ک</strong><strong>᫣ᒊ</strong><strong>ݷ</strong><strong>ਁӾ</strong><strong>ڊ</strong><strong>ሿེහ๋ग़ጱ୏१ਁҁ</strong><strong>ݢ</strong><strong>ᚆํग़ӻ҂̶</strong>ֺই҅੒ܖઊ܄ᵱᥝತکಅ ํܖԭ֖ઊ܄ጱࣈ᱈ᒊ҅ଚᕹᦇݷਁӾᒫӞӻਁڊሿጱེහ҅ଚਖ਼๋ग़ེහ੒ଫጱ܄ҁdistrict҂̵ਁ ҁchr҂̵ེහҁcntᬌ҂ڊ̶

ғӞᐏ൉ݶ໏೪ᶪ֕ਁ୵ӧݶጱਁӧᦊԅฎݶ໏ጱਁ̶

ྦྷਁӾପഝහғԫᐏ൉܄ҁdistrict҂ԅnullᕑӧᅩᒊጱفᘍᡤ̶

ၥᦶ෸஺ኼഭଧᳯ᷌

<strong>Sample Output:</strong>

<table width="629">

 <tbody>

  <tr>

   <td width="298"><strong>district</strong></td>

   <td width="166"><strong>chr</strong></td>

   <td width="165"><strong>cnt</strong></td>

  </tr>

  <tr>

   <td width="298">Bao’an</td>

   <td width="166">ਪ</td>

   <td width="165">4</td>

  </tr>

  <tr>

   <td width="298">Futian</td>

   <td width="166">ᐰ</td>

   <td width="165">4</td>

  </tr>

  <tr>

   <td width="298">Futian</td>

   <td width="166">܏</td>

   <td width="165">4</td>

  </tr>

  <tr>

   <td width="298">Futian</td>

   <td width="166">ḕ</td>

   <td width="165">4</td>

  </tr>

  <tr>

   <td width="298">Longgang</td>

   <td width="166">य़</td>

   <td width="165">2</td>

  </tr>

  <tr>

   <td width="298">Longhua</td>

   <td width="166">ὄ</td>

   <td width="165">2</td>

  </tr>

  <tr>

   <td width="298">Longhua</td>

   <td width="166">࿆</td>

   <td width="165">2</td>

  </tr>

  <tr>

   <td width="298">Luohu</td>

   <td width="166">ᕁ</td>

   <td width="165">2</td>

  </tr>

  <tr>

   <td width="298">Nanshan</td>

   <td width="166">Ⴎ</td>

   <td width="165">5</td>

  </tr>

 </tbody>

</table>


