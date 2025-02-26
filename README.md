# bash
- for a in 7 8 9; do for b in 2 3 6; do for c in 1 2 4; do for d in 1 2 3; do for e in 1 2 3; do for f in 2 3 6; do seq ${a}${b}${c}${d}${e}${f}0000 ${a}${b}${c}${d}${e}${f}9999 >> filtered_10digit_numbers.txt; done; done; done; done; done; done
- while read -r password; do echo "Trying: $password" >> attempts.log; unzip -tP "$password" Documents.zip >/dev/null 2>&1 && echo "Password found: $password" >> success.log && break; done < all_10digit_numbers.txt
