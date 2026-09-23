# Through the Ages (TTA) Probability Calculator 🎲
*(Scroll down for English version)*

這是一個專為知名桌遊《歷史巨輪 (Through the Ages)》設計的機率計算工具。它可以幫助你計算在特定時代中，對手（或你自己）抽到軍事關鍵牌（如侵略、戰爭、陣型等）的機率，並完美支援貝氏更新（扣除你已經知道的資訊）。

網頁採用響應式設計，沒有任何伺服器後端，非常適合在 iPad 或手機瀏覽器上直接加入主畫面當作 Web App 使用。

## 💡 使用說明與變數定義

計算器內建了 2人局與 3/4人局 的牌庫張數預設值。點擊上方按鈕，系統會自動幫您填入該時代對應的總牌數。

*   **N (牌庫原始總張數):** 該時代開始時，軍事牌庫的總張數。
*   **k (關鍵牌總張數):** 該時代中，你關心的目標牌（如所有侵略牌）的總數。
*   **p (你已看過的牌數):** 從該時代開始至今，你總共抽了幾張軍事牌，加上對手已經打在場上的牌。
*   **q (你看到的關鍵牌數):** 在你已經看過的牌中，有幾張是關鍵牌。
*   **m (抽幾張牌):** 對手這回合抽了幾張未知的牌（或者你預計自己即將抽幾張牌）。
*   **n (至少有幾張關鍵牌):** 你想計算「至少抽到幾張」的機率（通常為 1）。

### 📝 實戰範例 (TW)

**情境 1：防範對手的侵略**
> 在四人局的 **Age II (二時代)**，你很擔心對手手上有「Aggro (侵略)」。
> 你自己這回合抽了 **3** 張軍事牌，發現裡面剛好有 **1** 張侵略牌。
> 對手回合時，他消耗了所有紅點，一次抽了 **4** 張軍事牌。
*   **操作方式：**
    *   選擇 `4 人局` > `Age II` > `Aggro` (系統自動填入 N=56, k=9)
    *   你已看過的牌數 (p) = `3`
    *   你看到的關鍵牌數 (q) = `1`
    *   抽幾張牌 (m) = `4`
    *   至少有幾張關鍵牌 (n) = `1`
*   **結果：** 點擊計算，即可知道對手手中扣留侵略牌的威脅機率！

**情境 2：自己想抽陣型**
> 在兩人局的 **Age I (一時代)**，你急需一張陣型牌。
> 你自己之前已經抽了 **2** 張牌，都沒有陣型。
> 你下回合預計可以抽 **3** 張牌，你想知道抽中陣型的機率是多少？
*   **操作方式：**
    *   選擇 `2 人局` > `Age I` > `陣型` (系統自動填入 N=48, k=10)
    *   你已看過的牌數 (p) = `2`
    *   你看到的關鍵牌數 (q) = `0`
    *   抽幾張牌 (m) = `3`
    *   至少有幾張關鍵牌 (n) = `1`
*   **結果：** 這就是你下回合能成型的數學期望值。

---

# Through the Ages (TTA) Probability Calculator 🎲 (English)

A lightweight web-based probability calculator designed for the board game *Through the Ages: A New Story of Civilization*. It helps you calculate the exact probability of drawing specific military cards (Aggressions, Wars, Tactics, etc.) using Hypergeometric Distribution and Bayesian Updating (factoring in the cards you have already seen).

The UI is fully responsive and client-side only. You can easily add it to your iPad or smartphone's home screen as a standalone Web App.

## 💡 How to Use & Variables

The calculator includes built-in presets for 2-player and 3/4-player deck distributions. Simply click the preset buttons to auto-fill the initial deck sizes.

*   **N (Initial Deck Size):** The total number of military cards at the beginning of the Age.
*   **k (Total Key Cards):** The total copies of the specific card type (e.g., all Aggression cards) in that Age.
*   **p (Cards you have seen):** Total military cards you have drawn, plus any military cards already played face-up on the table by opponents.
*   **q (Key cards you have seen):** How many of those seen cards were the key cards you are tracking.
*   **m (Cards to draw):** The number of unknown cards your opponent just drew (or the number of cards you are about to draw).
*   **n (At least X key cards):** Your target condition. Usually `1` (probability of drawing at least 1 key card).

### 📝 Examples (EN)

**Scenario 1: Defending against Aggression**
> In a 4-player game during **Age II**, you are worried about an opponent holding an Aggression.
> You drew **3** military cards this turn, and **1** of them was an Aggression.
> On the opponent's turn, they drew **4** military cards.
*   **How to input:**
    *   Select `3/4 Players` > `Age II` > `Aggress` (Auto-fills N=56, k=9)
    *   Cards you have seen (p) = `3`
    *   Key cards you have seen (q) = `1`
    *   Cards to draw (m) = `4`
    *   At least X key cards (n) = `1`
*   **Result:** Click calculate to see the exact probability of the threat!

**Scenario 2: Drawing a Tactic for yourself**
> In a 2-player game during **Age I**, you desperately need a Tactic card.
> You have already drawn **2** cards previously, neither were Tactics.
> Next turn, you plan to draw **3** cards.
*   **How to input:**
    *   Select `2 Players` > `Age I` > `Tactic` (Auto-fills N=48, k=10)
    *   Cards you have seen (p) = `2`
    *   Key cards you have seen (q) = `0`
    *   Cards to draw (m) = `3`
    *   At least X key cards (n) = `1`
*   **Result:** You will see the probability of successfully finding a tactic next turn.
