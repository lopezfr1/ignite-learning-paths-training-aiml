# <a name="aiml20-speaker-notes"></a>AIML20：演講者備忘稿

如果您希望使用項目符號要點，而不使用底稿，以下是 PPT 簡報每一張投影片的重點：[presentations.md](https://github.com/microsoft/ignite-learning-paths-training-aiml/blob/master/aiml20/presentations.md)

您可以在 https://github.com/microsoft/ignite-learning-paths-training-aiml/tree/master/aiml20 找到相關聯的示範底稿。 請從 `DEMO%20Setup.md` 開始。

## <a name="slide-notes"></a>投影片備忘稿

投影片只會以標題識別。

### <a name="slide-microsoft-ignite-the-tour"></a>投影片：Microsft Ignite the Tour

簡報前的簡介投影片

### <a name="slide-using-pre-built-ai-to-solve-business-problems"></a>投影片：使用預先建立的 AI 解決商務問題

進行自我介紹。

如何將 AI 功能新增至應用程式，即使是在沒有計算資源或 AI 專業知識的情況下。

使用雲端中預先建立的 AI 服務。

### <a name="slide-resources"></a>投影片：資源

我們會提供許多連結、資源和示範。

所有項目的連結，包括完整原始程式碼與應用程式的單鍵部署，都位於此處的連結。

這張投影片會在結束時再次顯示。

### <a name="slide-adding-humanlike-capabilities-to-apps"></a>投影片：將擬人化功能新增至應用程式

我們將使用預先建立的 AI 服務，將擬人化功能新增至應用程式，但這是什麼意思？ 請看這些範例。

### <a name="slide-enhance-apps-with-humanlike-capabilities"></a>投影片：增強具有擬人化功能的應用程式

[按一下] 為您的應用程式提供語音功能 (例如聊天)。
 
[按一下] 讓您的應用程式能夠查看 (了解影像)。

[按一下] 為應用程式提供人類行為的直覺 (調整介面)。

[按一下] 為您的應用程式提供理解能力 (以任何語言溝通)

[按一下] 將執行掃描異常資料流的人工程序自動化 (以及規模)

這只是部分範例。

### <a name="slide-overview-of-azure-cognitive-services"></a>投影片：Azure 認知服務概觀

實施擬人化 AI 不是需要很多資料和很多技術專業知識嗎？

不需要。 根據 Microsoft Research 的專業知識來繪製。 使用簡單的 REST API 呼叫來新增功能。 

這就是 Azure 認知服務。

### <a name="slide-azure-cognitive-services"></a>投影片：Azure 認知服務

Azure 認知服務包含數十個 API。

這些擬人化功能類別內的服務包含：

視覺：了解相片、圖畫、文字和手寫以及影片的內容

語音：了解和辨識語音，並產生自然擬人化語音的工具。

語言：了解書面文件和文字的內容，並在人類語言之間互譯。

決策：Azure 認知服務的全新類別，就資料、內容和應用程式使用者介面做出擬人化選擇。

搜尋：回答以自然語言詢問的大型非結構化存放庫內容相關問題。 

### <a name="slide-azure-cognitive-services-with-service-names"></a>投影片：Azure 認知服務 (具有服務名稱)

我們已經討論過「搜尋」了。 

我們會另外使用一些可用的服務來增強零售網站：[按一下]

電腦視覺：用於分析產品相片的內容。

自訂視覺：用於找出零售商銷售的特定產品。

個人化工具：用於自動調整網站的版面配置 

但對所有 API 而言，設定和使用認知服務的原則都相同；因此，您今天在這裡所學到內容一體適用於您想要使用的任何 AI 服務。

### <a name="slide-computer-vision"></a>投影片：電腦視覺

首先，讓我們看看為電腦視覺預先建立的 AI。

### <a name="slide-shop-by-photo"></a>投影片：依相片購物

這是硬體零售商 Tailwind Traders (虛構公司) 的網站。 

### <a name="slide-demo-shop-by-photo"></a>投影片：示範：依相片購物

示範：「定義問題：依相片購物已中斷」

### <a name="video-shop-by-photo"></a>影片：依相片購物

讓我們前往實際的 Tailwind Traders 網站。 [按一下]

其中一項啟用 AI 的功能稱為「依相片購物」。 這項功能可讓客戶上傳想要購買的產品相片，而應用程式會告訴客戶有沒有這項產品。 讓我們立刻試試看。 我們將上傳這張我們感興趣的電鑽圖片，接著 Tailwind Traders 應用程式會分析圖片來辨識出這是電鑽，並向我顯示 Tailwind Traders 有這項產品待售，且告訴我其位在店裡的哪個位置。

但讓我們試試另一張圖片。 我回到首頁，再次使用「依相片購物」功能，這次選擇這張鉗子的圖片。 很不幸，應用程式分析圖片時，以為這是把鐵錘。 顯然效果不彰，所以我們來看看能不能找出問題，使用電腦視覺找到修正的方法。 

### <a name="slide-how-computer-vision-works"></a>投影片：電腦視覺的運作方式

我們現在來討論一下理論。 沒有很多數學。

有助於了解可能發生錯誤的地方，以及如何修正問題。

### <a name="slide-tasks-xkcd-comic"></a>投影片：工作 (XKCD 漫畫)

(暫停 10 秒鐘)

能夠理解相片的電腦，在過去只會出現在科幻小說裡。

現在過了 5 年，這不只是可行而已，還很簡單。

### <a name="slide-how-neural-networks-work-brandon-rohrer"></a>投影片：神經網路的運作方式 (Brandon Rohrer)

經 Brandon Rohrer 授權改編。

請查看他的影片教學課程系列部落格，其包含 AI 和機器學習服務許多層面的深入說明。 

### <a name="slide-computer-vision--convolutional-neural-network"></a>投影片：電腦視覺/卷積神經網路

AI 採用「深度學習」技術，但「深度」並不代表「深奧」。

這是簡單的神經網路。 真實世界的神經網路會有更多層。

其設計目的是要偵測五個物件。 無法辨識其他任何項目。

### <a name="slide-trained-convolutional-nn"></a>投影片：經訓練的卷積神經網路

輸入影像會位於左側。 

每個節點會處理和重新結合原始影像並將其縮小，直到最後為單一值：分類信賴度。

此處的輸入是自行車，且右側具有最大值的節點為「自行車」。 這張影像已正確識別。

### <a name="slide-filters-1"></a>投影片：篩選器 (1)

略過以節省時間。

### <a name="slide-filters-2"></a>投影片：篩選器 (2)

略過以節省時間。

### <a name="slide-filters-3"></a>投影片：篩選器 (3)

略過以節省時間。

### <a name="slide-training-an-image-classifier"></a>投影片：訓練影像分類器

但是，您要如何訓練神經網路來這麼做？

[按一下] 選擇正確的篩選器。 每個篩選器都由權數小方格 (通常是 3x3 或 5x5) 所控制。

[按一下] 我們會使用已知分類的大量訓練影像來選擇權數。 選擇權數以選擇正確的分類 (或至少大部分的時間都正確)

在真正的視覺網路中，可能有數百萬個權數要選擇。 如何判斷權數？

### <a name="slide-learning-backpropagation"></a>投影片：學習：反向傳播

這裡就需要大量的數學了。

但除非您是 AI 工程師，否則不用在意。 您可以直接使用已由其他人將權數最佳化的網路。

這涵蓋了 80% 的應用程式。 但是，如果您需要設計自己的神經網路並將權數最佳化，您可以利用 Tensorflow 和 PyTorch 等工具。 您可以在 AIML40 和 AIML50 中了解相關資訊。

### <a name="slide-pre-trained-convolutional-nn"></a>投影片：訓練前的卷積神經網路

但是，只要您能存取可偵測所需影像的神經網路，那麼您只需要提供影像，讓網路為您分類即可。

有些模型不僅執行分類，也會偵測物件位置，或以其他方式分析影像。

### <a name="slide-demo-cognitive-services-computer-vision"></a>投影片：示範：認知服務電腦視覺

認知服務電腦視覺提供功能強大的神經網路，可以分類數千個物件。

您可以在 aka.ms/try-computervision 試用一個簡單的 Web 型 UI

讓我們立即試試看。

### <a name="video-computer-vision-via-web"></a>影片：透過 Web 的電腦視覺

[按一下] 這是認知服務的電腦視覺頁面。 將該頁面稍微向下捲動一點，您會看到一份不錯的 Web 表單，其讓我們可以從 Web 或本機檔案上傳影像以供分析。 所以，讓我們試著上傳這張戴著安全帽的男人圖片。 只要幾秒，我們就會收到電腦視覺服務對該圖片的分析。 左邊是在影像中偵測到的物件，右邊則是附詳細分析的 JSON 輸出。 其中包括在影像中偵測到的物件名稱和位置、與影像建立關聯的標記或標籤清單、對影像的一般語言描述 (在此案例中為「戴著頭盔的男人」)，以及其他許多有用的資訊。

### <a name="slide-cognitive-services-computer-vision"></a>投影片：認知服務電腦視覺

查看物件：偵測到兩個物件。 帽子和人。

查看標記。 信賴度最高：男人。 下一個是「頭巾」。 頭盔只位於第 6。
模型並未特別針對「安全帽」來訓練。

我們等一下會了解如何修正此問題。

如果您希望將視覺納入應用程式，您可以程式設計方式來存取 API。 讓我們看看怎麼做。

### <a name="video-computer-vision-via-cli"></a>影片：透過 CLI 的電腦視覺

您可以使用能夠連線到 HTTP 端點的任何語言來連接到認知服務 API，而我在這裡用的 [按一下] 是 bash 指令碼，這種指令碼使用 Azure CLI 建立資源，並使用 "curl" 連線到電腦視覺 API。 您可以在本機殼層中安裝 Azure CLI，但我在這裡使用 Visual Studio Code 的「Azure 帳戶」延伸模組來啟動 Cloud Shell，這表示我不用進行任何安裝。 一旦該殼層就緒，我就可以從這個 bash 指令碼直接執行命令。 

第一個命令會建立一個資源群組，用來保存驗證 API 所需的金鑰。

下一步是建立金鑰。 我在這裡建立可用於許多服務的綜合性認知服務金鑰，包括電腦視覺。

然後，我們可以直接在終端中顯示金鑰。 [等待] 您可以使用這兩個金鑰的其中一個來連接 API，在此，我會將第一個金鑰儲存在環境變數中。

我們可使用該金鑰來連線到電腦視覺服務所提供的端點 URL，因此，我們也將該 URL 儲存在環境變數中。

然後您可以選擇一張影像來加以分析。 我們在此提供一個影像的 URL，即剛才所看到戴著安全帽男人的同一影像。

現在，我們可以使用 curl 藉由傳入 JSON 輸入將金鑰和影像 URL 傳入端點。 只要幾毫秒，我們就會收到該影像的 JSON 分析。 您會看到剛才我們在 Web 介面中看到的相同輸出。

當然，我們可以對任何影像執行這項作業。 讓我們對另一張影像再執行一次這項作業，這次用電鑽的圖片。 同樣地，我們可以使用 curl 將圖片傳到 API。 [等待] 有趣的是，與此影像建立關聯的最上層標記是「相機」，這當然沒辦法幫助我們搜尋真正的工具，我們想要的是「電鑽」。

### <a name="slide-adapting-computer-vision-models-with-your-own-data"></a>投影片：使用您自己的資料調整電腦視覺模型

電腦視覺 API 不適用於「相機」。 

已經訓練成偵測太多類型的物件了。

所幸，我們可以修正該問題。 讓我們回顧一下此理論。

有一種方式可以調整數千個物件的模型，能將其調整成只偵測您想要的物件。 即使這些物件不是原始模型的一部分。 

我們來看一下如何使用稱為「轉移學習」的 AI 技術。 

### <a name="slide-transfer-learning"></a>投影片：轉移學習

如同先前的卷積神經網路，但移除了最後一個層。

第二層會提供「功能」，您可以將其視為數字的向量。 每個影像都會產生一組不同的功能。

我們並不知道這些功能所代表的內容，但其對於分類影像而言很有幫助。

訣竅：我們可以使用這些功能來分類一組新的物件。

### <a name="slide-transfer-learning-training-1---with-the-hammer"></a>投影片：轉移學習訓練 (1 - 使用鐵錘)

使用「轉移學習」建立模型以識別鐵鎚與安全帽。

傳遞鐵鎚的圖片並收集功能。 以及「鐵鎚」的二元指標。 重複此動作來傳遞大量鐵鎚的圖片。

### <a name="slide-transfer-learning-training-2---with-the-white-hard-hat"></a>投影片：轉移學習訓練 (2 - 使用白色安全帽)

現在，對安全帽的圖片執行相同作業。

在每個案例中，收集每個影像的 8 個資料向量和二元指標。

全部整合在一起，可獲得資料向量的集合，每個向量都有相關聯的二元結果。 

您即可據以建立簡單的預測模型。

### <a name="slide-transfer-learning-trained-model"></a>投影片：轉移學習的訓練模型

運作得非常順利。

您不需要大量影像或運算能力。

這只是個小小的範例，但準則也同樣適用於大型模型。

### <a name="slide-microsoft-cognitive-services-custom-vision"></a>投影片：Microsoft 認知服務自訂視覺

當然，您不必自行訓練轉移學習模型。

使用其中一種 Microsoft 預先訓練的視覺模型，並透過自訂視覺以您自己的物件影像來調整模型。

讓我們試試用這個模型來建立依相片購物的視覺模型。

### <a name="slide-demo-customized-object-recognition"></a>投影片：示範：自訂物件辨識

示範指示： https://github.com/microsoft/ignite-learning-paths-training-aiml/blob/master/aiml20/DEMO%20Custom%20Vision.md

### <a name="video-customvisionai"></a>影片：customvision.ai

[按一下] 我現在位於自訂視覺 Web 介面。 此介面提供很棒的 UI，我們可在此提供新的影像，供轉移學習分析之用。 而且您可以在這個專案中看到，我已經上傳了一些圖片。 我上傳了螺絲起子、鉗子、電鑽和鐵槌的圖片，我要用這些圖片來訓練我的自訂模型。 我們也想偵測 Tailwind Traders 銷售的另一項產品：安全帽。 所以，我們按一下 [新增影像]，瀏覽到硬碟資料夾，我在這裡收集了一些安全帽圖片，全部選取後將這些圖片新增至服務，同時提供「安全帽」標籤用於訓練。

上傳這些檔案需要一點時間，但在執行這項作業時請注意，這個專案沒有那麼多的影像：共約 180 張，或五個類別的每一個有數十張。 有時還更少。 儘管如此，因為我的五個物件類型為完全相異，所以模型的效果應該相當不錯。

那麼，繼續作業，按一下 [訓練] 按鈕開始轉移學習。 我們選擇 [快速訓練]。 現在，快速訓練正在透過複雜的視覺模型掃描所有影像，並使用轉移學習來建立五個類別的預測模型。 只需要花幾秒鐘，模型運作得相當不錯！
機率閾值會設定一個限制，低於此限制就完全預測不出任何分類。 如果我們只接受信賴度為 50% 或以上的分類，則這些預測 90.9% 為正確：這是「精確度」。 而模型正確分類全部影像的 88.2%：這是「重新叫用」。 在應用程式中，您將根據建立錯誤呼叫與完全不建立呼叫的容錯來選擇閾值。 我們可以為 Tailwind Traders 設定偏低的閾值，因為向客戶建議錯誤的產品沒什麼大不了。 但如果這是癌症偵測應用程式，您可能要建立不同的呼叫。

現在，讓我們用一些模型沒有見過的新影像試試。 按一下 [快速測試] 按鈕即可。 我們會從 [test images] 資料夾上傳新的檔案。 讓我們試試戴著安全帽的男人。 您可以看到，我們的預測確實是「安全帽」，且機率為 99.9%，所以選擇任何閾值應該都能叫出這個結果。

再試試不同的影像：電鑽。 模型將此影像識別為電鑽的機率為 94.5%。 最後，試試鉗子的圖片，識別信賴度為 99.9%。

雖然訓練的影像不到 200 張，但我們的模型運作效能良好。
這是因為我們將可能標籤限制於僅在 Tailwind Traders 銷售的產品。

現在模型沒問題了，我們就可以匯出模型並將其併入應用程式。 如果您按一下 [匯出] 按鈕，就可以容器形式或此案例中的通用 ONNX 格式，匯出適用於 iOS 或 Android 的模型。 現在我們已將此模型下載到硬碟。

### <a name="slide-portable-deep-learning-models"></a>投影片：可攜式深度學習模型

我們以 ONNX 格式匯出自訂模型。

ONNX (Open Neural Network Exchange) 是 Microsoft 和 Facebook 所推出的開放式標準，旨在推廣免費交換和部署 AI 模型，受到眾多應用程式和技術廠商的支援。

我們已使用 ONNX Runtime 將匯出的模型整合至網站。

### <a name="slide-onnximagesearchtermpredictorcs"></a>投影片：ONNXImageSearchTermPredictor.cs

InferenceSession 意指匯出的 .onnx 檔案

模型會產生分類標籤，並將其傳遞給搜尋。

### <a name="slide-demo-onnx"></a>投影片：示範：ONNX

示範：ONNX 部署

### <a name="video-kudu"></a>影片：Kudu

[按一下] 我們剛才從自訂視覺匯出的模型其實是一個 ZIP 檔案，包含實際的 ONNX 檔案 model.onnx，這是剛才所建立神經網路的文字表示，也是資訊清單檔。 

現有的 Tailwind Traders 網站已使用電腦視覺模型，這會以稱為 products.onnx 的 ONNX 檔案表示。 問題是，該模型不能正確識別在 Tailwind Traders 銷售的許多產品。 因此，我們將剛才從自訂視覺匯出的 model.onnx 檔案重新命名為 products.onnx，並以此取代 Web 應用程式中的檔案，讓「依相片購物」可以識別我們訓練模型所用的所有五項產品。

在這個 Azure 入口網站中，您可以看到執行 Tailwind Traders 網站的 App Service 資源。 我現在可以在 App Service 中前往 [開發工具] 區段並選擇 [進階工具] 功能。 這會啟動 Kudu 介面。 介面啟動後，我就可以使用偵錯主控台來瀏覽網站的檔案系統。 讓我們瀏覽至 site、w-root、Standalone、OnnxModels，這是 products.onnx 檔案所在的位置。 現在我們可以用以自訂視覺建立的新版 products.onnx 檔案取代這個檔案。

現在我們可以回到 App Service 繼續作業，重新啟動網頁伺服器，讓伺服器在「依相片購物」功能中使用新的 ONNX 模型。

### <a name="video-netron"></a>影片：Netron

[按一下] 在等待網站重新啟動時，我們先來看看剛才安裝的 ONNX 模型內部。 有一個 Lutz Roeder 製作的小型 Web 應用程式很好用，稱為 Netron，能讓我們檢查 ONNX 檔案中的神經網路。 接著繼續開啟這個 products.onnx 檔案。 在此您可以看到模型呈現的實際神經網路層。 放大一點，看一下最上層的輸入。 該輸入是一張影像。 這是 3 層的 RGB 影像，大小為 224x224 像素。 我必須實際裁剪縮小使用者提供的影像，才能將影像提供給 ONNX Runtime。 說出來有點不好意思，電腦視覺系統的視力其實很糟糕，其使用的影像解析度相當低，不過工作能力還是很好的。

現在放大，然後向下捲動網路。 您可以看到自訂視覺所建立神經網路中的所有層，每一層都會轉換輸入影像、套用篩選並重新合併輸出影像，正如您在此討論稍早所了解。 但到達最後一層的輸出層時，您會看到輸出為五個值的清單，即我們訓練模型所用的五項產品：鐵槌、安全帽等，以及標示為 "loss" 的這個值，這是模型預測每個類別的信賴度。 在應用程式中，您要選擇自己的閾值以決定信賴度高低。

不管怎樣，現在 Tailwind Traders 網站已重新啟動，讓我們回到首頁看看新的視覺模型運作得如何。 好，繼續上傳相片，再試一次其中一張測試影像，特別是之前不成功的鉗子影像。 我們可以看到網站不認為這是鐵槌，其搜尋了「鉗子」並顯示所有提供的產品。

### <a name="slide-optimizing-app-ui-with-cognitive-services-personalizer"></a>投影片：使用認知服務個人化工具將應用程式 UI 最佳化

接下來是一個更快速的範例：個人化工具。

「個人化工具」服務可讓我們從使用者行為中學習，即時自訂應用程式的介面。

### <a name="slide-recommended-screenshot"></a>投影片：建議 (螢幕擷取畫面)

建議區段顯示一張大的「主要」影像，加上幾張較小的影像。

個人化工具會選取要讓區段顯示的順序

使用一項稱為「增強式學習」的 AI 技術。

### <a name="slide-personalizer-in-action"></a>投影片：作用中的個人化工具

Microsoft 花了數年時間開發個人化工具。 

用於 XBox、Bing 和 MSN 新聞。

現在您也可以在自己的應用程式中使用個人化工具。

### <a name="slide-reinforcement-learning"></a>投影片：增強式學習

個人化工具實作一項稱為增強式學習的 AI 技術。 其運作方式如下。

[按一下] 假設我們想要向使用者顯示「主要」動作。 [按一下] 使用者可能不確定接下來該做什麼，[按一下] 但我們可以顯示數項建議的其中之一。 在遊戲應用程式中，[按一下] 可能是：「玩遊戲」、「看電影」或「加入公會」。 [按一下] 根據使用者的歷程記錄和其他內容資訊 (例如其位置、一天的時段、星期幾)，個人化工具服務會 [按一下] 列出可能動作的排位，[按一下] 建議最應該升階的動作 [按一下]。 

我們當然希望使用者滿意 [按一下]，可是怎麼確定呢？ 這取決於使用者接下來會做什麼，以及這是否為我們希望使用者會做的事。
根據我們的商務邏輯 [按一下]，我們會為接下來發生的事指派 0 到 1 的「獎勵分數」。 例如，花更多時間玩遊戲或讀一篇文章，或在商店花更多錢，可能得到更高的獎勵分數。 [按一下] 當我們下次需要主打某項活動時，個人化工具會將此資訊饋送回排名系統。

### <a name="slide-discovering-patterns-and-causality"></a>投影片：探索模式與因果關係

不僅僅是個建議系統。

探索模式會以您指定的速率來呈現其他選項。

就像是即時的 A/B 測試。

### <a name="slide-personalizer-for-tailwind-traders"></a>投影片：Tailwind Traders 的個人化工具

內容：一天的時段、星期幾、瀏覽器 OS  

獎勵分數：如果按下精選分類則為 1，否則為零。

探索速率：20%

### <a name="slide-demo-personalizer"></a>投影片：示範：個人化工具

[按一下] 現在，讓我們來看看作用中的個人化工具。 回到 Tailwind Traders 首頁。 之前沒有提到，在這個 [建議] 區段中，產品部門的排序是由個人化工具決定。
在此案例中，顯示的主要影像是電器部門。 如果重新整理網站幾次，也會看到「探索」行為。
顯然，使用我在這裡所用的瀏覽器和作業系統，個人化工具認為在一天的這個時段中，園藝中心會取得最好的匿名使用者參與表現，但最後還是會嘗試不同的類別，這裡會跳出連接，而個人化工具也會用此來評量參與程度。

### <a name="slide-pre-built-ai-in-production"></a>投影片：生產環境中預先建立的 AI

總結一下將 AI 放入生產環境時的一些考量。

### <a name="slide-cost-considerations"></a>投影片：成本考量

第一個考量：成本。 

不熟悉 Azure 嗎？ 使用此連結註冊，可獲得美金 $200 元的免費點數。

[按一下] 開發規模的工作負載通常免費 

[按一下] 從生產環境磁碟區開始會收費

[按一下] 此連結提供依服務和區域的特定詳細資料

### <a name="slide-data-considerations"></a>投影片：資料考量

想想看，自己的資料去了哪裡、用於什麼樣的用途。

資料會上傳以進行推斷，但在使用之後會立即刪除。 此連結提供詳細資料。

如果頻寬不足，或資料受到規範限制，請考慮使用容器。

### <a name="slide-deployment-with-containers"></a>投影片：使用容器的部署

可下載的容器可提供一些服務。

在您的防火牆後方安裝容器，就不會將任何資料傳送給 Microsoft。

網際網路連線僅用於計費。 以一般費率收費。

### <a name="slide-ethical-considerations"></a>投影片：道德考量

最重要的投影片。

了解 AI 應用程式會對人員造成影響的道德含意。

符合道德的架構應該要：

「賦予人員能力」  ，讓其能在已經進行的事項中達成更多目標 (不要取代人員)

能「包容」  所有類型的使用者：務必讓所有人都能公平得益於您的應用程式；以及

保持公平與透明。

請記住，只有用來訓練 AI 的資料夠好，AI 才會運作得好。 請確保應用程式適用於所有潛在使用者。

如果您尚未設定道德架構，請利用 Microsoft 的人工智慧原則，更多資訊請參閱此連結。

### <a name="slide-wrapping-up"></a>投影片：結語

預先建立的模型並非萬能，但可以讓您快速取得進展。 

AI 是由資料所驅動。 請記住資料，以及可能發生錯誤的地方。

親自動手試試看！ 您不需要擁有大量的專業知識，但仍需考量道德含意。

### <a name="slide-docs-alert"></a>投影片：Docs 提醒

如需 Azure 認知服務的所有詳細資料，包括快速入門指南和參考，請參閱 Microsoft Docs。

### <a name="slide-ms-learn-alert"></a>投影片：MS Learn 提醒

如果想要了解如何使用認知服務，Microsoft Learn 有免費課程可逐步引導您使用該服務。

### <a name="slide-resources"></a>投影片：資源

所有連結與程式碼都位於此 Github 存放庫。

如果您想要取得 AI 或資料科學的 Microsoft 認證，出席者今天有免費認證的特殊優惠：詳細資料請參閱此連結。

我會在這裡回答問題。 (以及...)

謝謝。