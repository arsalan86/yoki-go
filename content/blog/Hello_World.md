---
title: "Hello World"
desrcription: "I've got this up and running!"
categories: ["general"]
tags: ["static", "Hugo", "rust", "hello world"]
date: 2017-07-29T13:49:30+05:00
draft: false
---

It Works!


This is a block of text it is a bloc of text it is still a block of text what am i doing please stop me please!
This is a block of text it is a bloc of text it is still a block of text what am i doing please stop me please!
This is a block of text it is a bloc of text it is still a block of text what am i doing please stop me please!
This is a block of text it is a bloc of text it is still a block of text what am i doing please stop me please!
This is a block of text it is a bloc of text it is still a block of text what am i doing please stop me please!
This is a block of text it is a bloc of text it is still a block of text what am i doing please stop me please!
This is a block of text it is a bloc of text it is still a block of text what am i doing please stop me please!
This is a block of text it is a bloc of text it is still a block of text what am i doing please stop me please!
This is a block of text it is a bloc of text it is still a block of text what am i doing please stop me please!
This is a block of text it is a bloc of text it is still a block of text what am i doing please stop me please!

pub


>$ sudo apt-get install build-essential

    INLINE BLOCK INLINE BLOCK
    INLINE BLOCK INLINE BLOCK     ruin ur formattingz
    INLINE BLOCK INLINE BLOCK                  all of ur formattingz
    INLINE BLOCK INLINE BLOCK
    INLINE BLOCK INLINE BLOCK
    def

    pub pub

```
    #[derive(Serialize, Deserialize)]
    pub struct ConfigFile {
        pub filepath: String,
        pub blake2hash: String,
        pub comment: String,

    }

    impl ConfigFile {
        pub fn get_hash(&mut self) -> Result<String, io::Error> {

            let data = read_file(&self.filepath)?;
            let mut hasher = Blake2b::default();
            hasher.input(&data.into_bytes());
            let output = String::from(format!("{:x}", hasher.result()));
            Ok(output)
        }

        pub fn check_hash_changed(&mut self) -> bool {

            let oldhash = self.blake2hash.clone();
            self.blake2hash = self.get_hash().unwrap();
            oldhash != self.blake2hash
        }

        pub fn get_contents(&self) -> String {

            read_file(&self.filepath).unwrap()

        }

    }
```