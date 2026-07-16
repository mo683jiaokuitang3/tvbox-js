import cheerio from 'assets://js/lib/cheerio.min.js';

const appConfig = {
    siteName: "GiriGiri爱",
    siteUrl: "https://ani.girigirilove.com"
};
const UA = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36";

const classList = [
    { type_id: "2", type_name: "日番" },
    { type_id: "3", type_name: "美番" },
    { type_id: "20", type_name: "真人番劇" },
    { type_id: "21", type_name: "劇場版" },
    { type_id: "24", type_name: "BD副音軌" },
    { type_id: "26", type_name: "演唱會&其他" }
];

const genreList2 = [
    { n: "全部", v: "" },
    { n: "喜剧", v: "喜剧" },
    { n: "爱情", v: "爱情" },
    { n: "恐怖", v: "恐怖" },
    { n: "动作", v: "动作" },
    { n: "科幻", v: "科幻" },
    { n: "剧情", v: "剧情" },
    { n: "战争", v: "战争" },
    { n: "奇幻", v: "奇幻" },
    { n: "冒险", v: "冒险" },
    { n: "悬疑", v: "悬疑" },
    { n: "校园", v: "校园" },
    { n: "后宫", v: "后宫" },
    { n: "热血", v: "热血" },
    { n: "运动", v: "运动" },
    { n: "职场", v: "职场" },
    { n: "百合", v: "百合" },
    { n: "乙女", v: "乙女" },
    { n: "机甲", v: "机甲" },
    { n: "日常", v: "日常" },
    { n: "魔法少女", v: "魔法少女" },
    { n: "异世界", v: "异世界" },
    { n: "爱抖露", v: "爱抖露" },
    { n: "音乐", v: "音乐" },
    { n: "萌", v: "萌" }
];

const genreList3 = [
    { n: "全部", v: "" },
    { n: "搞笑", v: "搞笑" },
    { n: "爱情", v: "爱情" },
    { n: "恐怖", v: "恐怖" },
    { n: "动作", v: "动作" },
    { n: "科幻", v: "科幻" },
    { n: "剧情", v: "剧情" },
    { n: "战争", v: "战争" },
    { n: "奇幻", v: "奇幻" },
    { n: "冒险", v: "冒险" },
    { n: "悬疑", v: "悬疑" },
    { n: "校园", v: "校园" },
    { n: "后宫", v: "后宫" },
    { n: "热血", v: "热血" },
    { n: "运动", v: "运动" }
];

const genreList20 = [
    { n: "全部", v: "" },
    { n: "喜剧", v: "喜剧" },
    { n: "爱情", v: "爱情" },
    { n: "恐怖", v: "恐怖" },
    { n: "动作", v: "动作" },
    { n: "科幻", v: "科幻" },
    { n: "剧情", v: "剧情" },
    { n: "战争", v: "战争" },
    { n: "奇幻", v: "奇幻" },
    { n: "冒险", v: "冒险" },
    { n: "悬疑", v: "悬疑" },
    { n: "校园", v: "校园" },
    { n: "后宫", v: "后宫" },
    { n: "热血", v: "热血" },
    { n: "运动", v: "运动" },
    { n: "职场", v: "职场" },
    { n: "百合", v: "百合" },
    { n: "乙女", v: "乙女" },
    { n: "机甲", v: "机甲" },
    { n: "日常", v: "日常" },
    { n: "魔法少女", v: "魔法少女" },
    { n: "异世界", v: "异世界" },
    { n: "爱抖露", v: "爱抖露" },
    { n: "音乐", v: "音乐" },
    { n: "萌", v: "萌" },
    { n: "纪录片", v: "纪录片" }
];

const genreList21 = [
    { n: "全部", v: "" },
    { n: "喜剧", v: "喜剧" },
    { n: "爱情", v: "爱情" },
    { n: "恐怖", v: "恐怖" },
    { n: "动作", v: "动作" },
    { n: "科幻", v: "科幻" },
    { n: "剧情", v: "剧情" },
    { n: "战争", v: "战争" },
    { n: "奇幻", v: "奇幻" },
    { n: "冒险", v: "冒险" },
    { n: "悬疑", v: "悬疑" },
    { n: "校园", v: "校园" },
    { n: "后宫", v: "后宫" },
    { n: "热血", v: "热血" },
    { n: "运动", v: "运动" },
    { n: "百合", v: "百合" },
    { n: "耽美", v: "耽美" },
    { n: "机甲", v: "机甲" },
    { n: "日常", v: "日常" },
    { n: "魔法少女", v: "魔法少女" },
    { n: "异世界", v: "异世界" },
    { n: "爱抖露", v: "爱抖露" },
    { n: "音乐", v: "音乐" }
];

const genreList24 = [
    { n: "全部", v: "" },
    { n: "喜剧", v: "喜剧" },
    { n: "爱情", v: "爱情" },
    { n: "恐怖", v: "恐怖" },
    { n: "动作", v: "动作" },
    { n: "科幻", v: "科幻" },
    { n: "剧情", v: "剧情" },
    { n: "战争", v: "战争" },
    { n: "奇幻", v: "奇幻" },
    { n: "冒险", v: "冒险" },
    { n: "悬疑", v: "悬疑" },
    { n: "校园", v: "校园" },
    { n: "后宫", v: "后宫" },
    { n: "热血", v: "热血" },
    { n: "运动", v: "运动" },
    { n: "百合", v: "百合" },
    { n: "乙女", v: "乙女" },
    { n: "机甲", v: "机甲" },
    { n: "日常", v: "日常" },
    { n: "魔法少女", v: "魔法少女" },
    { n: "异世界", v: "异世界" },
    { n: "爱抖露", v: "爱抖露" },
    { n: "音乐", v: "音乐" }
];

const quarterList = [
    { n: "全部", v: "" },
    { n: "一月", v: "一月" },
    { n: "四月", v: "四月" },
    { n: "七月", v: "七月" },
    { n: "十月", v: "十月" }
];

function makeYearList(from) {
    let years = [{ n: "全部", v: "" }];
    let cy = new Date().getFullYear();
    for (let y = cy; y >= from; y--) {
        years.push({ n: String(y), v: String(y) });
    }
    return years;
}

const sortList = [
    { n: "默认", v: "" },
    { n: "最新", v: "time" },
    { n: "最热", v: "hits" },
    { n: "评分", v: "score" }
];

const myFilters = {
    "2": [
        { key: "genre", name: "类型", value: genreList2 },
        { key: "quarter", name: "季度", value: quarterList },
        { key: "year", name: "年份", value: makeYearList(2010) },
        { key: "sort", name: "排序", value: sortList }
    ],
    "3": [
        { key: "genre", name: "类型", value: genreList3 },
        { key: "quarter", name: "季度", value: quarterList },
        { key: "year", name: "年份", value: makeYearList(2005) },
        { key: "sort", name: "排序", value: sortList }
    ],
    "20": [
        { key: "genre", name: "类型", value: genreList20 },
        { key: "quarter", name: "季度", value: quarterList },
        { key: "year", name: "年份", value: makeYearList(2010) },
        { key: "sort", name: "排序", value: sortList }
    ],
    "21": [
        { key: "genre", name: "类型", value: genreList21 },
        { key: "quarter", name: "季度", value: quarterList },
        { key: "year", name: "年份", value: makeYearList(2005) },
        { key: "sort", name: "排序", value: sortList }
    ],
    "24": [
        { key: "genre", name: "类型", value: genreList24 },
        { key: "quarter", name: "季度", value: quarterList },
        { key: "year", name: "年份", value: makeYearList(2005) },
        { key: "sort", name: "排序", value: sortList }
    ],
    "26": [
        { key: "genre", name: "类型", value: [{ n: "全部", v: "" }] },
        { key: "quarter", name: "季度", value: quarterList },
        { key: "year", name: "年份", value: makeYearList(2005) },
        { key: "sort", name: "排序", value: sortList }
    ]
};

function fixUrl(u) {
    if (!u) return '';
    if (u.startsWith('http')) return u;
    if (u.startsWith('//')) return 'https:' + u;
    if (u.startsWith('/')) return appConfig.siteUrl + u;
    return u;
}

const b64chars = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/=";
function base64decode(str) {
    let output = "";
    let chr1, chr2, chr3, enc1, enc2, enc3, enc4;
    let i = 0;
    str = str.replace(/[^A-Za-z0-9+/=]/g, "");
    while (i < str.length) {
        enc1 = b64chars.indexOf(str.charAt(i++));
        enc2 = b64chars.indexOf(str.charAt(i++));
        enc3 = b64chars.indexOf(str.charAt(i++));
        enc4 = b64chars.indexOf(str.charAt(i++));
        chr1 = (enc1 << 2) | (enc2 >> 4);
        chr2 = ((enc2 & 15) << 4) | (enc3 >> 2);
        chr3 = ((enc3 & 3) << 6) | enc4;
        output = output + String.fromCharCode(chr1);
        if (enc3 !== 64) output = output + String.fromCharCode(chr2);
        if (enc4 !== 64) output = output + String.fromCharCode(chr3);
    }
    return output;
}

function buildCategoryUrl(tid, pg, extend) {
    extend = extend || {};
    let genreVal = extend.genre ? encodeURIComponent(extend.genre) : '';
    let quarterVal = extend.quarter ? encodeURIComponent(extend.quarter) : '';
    let yearVal = extend.year || '';
    let sortVal = extend.sort || '';
    let pageVal = pg > 1 ? String(pg) : '';

    let parts = [
        tid,
        quarterVal,
        sortVal,
        genreVal,
        '',
        '',
        '',
        '',
        pageVal,
        '',
        '',
        yearVal
    ];
    return appConfig.siteUrl + '/show/' + parts.join('-') + '/';
}

function cleanEpisodeName(name) {
    if (!name) return "";
    return name
        .replace(/立即播放/g, "")
        .replace(/立即观看/g, "")
        .replace(/点击播放/g, "")
        .replace(/在线播放/g, "")
        .replace(/免费播放/g, "")
        .replace(/\s+/g, " ")
        .trim();
}

function parseListHtml(html) {
    const $ = cheerio.load(html);
    let list = [];
    let vodIds = {};

    $(".public-list-box.public-pic-b").each(function() {
        let $box = $(this);
        let $link = $box.find("a.public-list-exp").first();
        let href = $link.attr("href") || "";

        let idMatch = href.match(/\/GV(\d+)\//);
        if (!idMatch) return;
        let vod_id = "/GV" + idMatch[1] + "/";

        if (vodIds[vod_id]) return;
        vodIds[vod_id] = true;

        let vod_name = $link.attr("title") || "";
        if (!vod_name) {
            vod_name = $box.find("a.time-title").text().trim() || "";
        }

        let vod_pic = "";
        let $img = $link.find("img").first();
        if ($img.length > 0) {
            vod_pic = $img.attr("data-src") || $img.attr("src") || "";
        }
        vod_pic = fixUrl(vod_pic);

        let vod_remarks = "";
        let $note = $link.find(".public-list-prb").first();
        if ($note.length > 0) {
            vod_remarks = $note.text().trim();
        }

        if (vod_name && vod_id) {
            list.push({ vod_id, vod_name, vod_pic, vod_remarks });
        }
    });

    let pagecount = 1;
    let $pageTip = $(".page-tip");
    if ($pageTip.length > 0) {
        let tipText = $pageTip.text();
        let match = tipText.match(/当前\s*(\d+)\/(\d+)\s*页/);
        if (match) {
            pagecount = parseInt(match[2]) || 1;
        }
    }

    if (pagecount <= 1) {
        let $pageInfo = $(".page-info");
        if ($pageInfo.length > 0) {
            let maxPage = 0;
            $pageInfo.find("a.page-link").each(function() {
                let text = $(this).text().trim();
                if (/^\d+$/.test(text)) {
                    let p = parseInt(text);
                    if (p > maxPage) maxPage = p;
                }
            });
            if (maxPage > 0) pagecount = maxPage;
        }
    }

    if (pagecount <= 1 && list.length > 0) {
        pagecount = 1;
    }

    return { list, pagecount };
}

async function init(ext) {
    console.log("初始化爬虫:", appConfig.siteName);
}

async function home(filter) {
    let list = [];
    try {
        const html = (await req(appConfig.siteUrl, {
            method: "GET",
            headers: {
                "User-Agent": UA,
                "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8"
            }
        })).content;
        const result = parseListHtml(html);
        list = result.list;
    } catch (e) {
        console.error("首页推荐获取失败:", e.message);
    }

    return JSON.stringify({
        class: classList,
        filters: myFilters,
        list: list.slice(0, 30)
    });
}

async function category(tid, pg, filter, extend) {
    pg = pg || 1;
    extend = extend || {};

    let url = buildCategoryUrl(tid, pg, extend);

    try {
        const html = (await req(url, {
            method: "GET",
            headers: {
                "User-Agent": UA,
                "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8",
                "Referer": appConfig.siteUrl
            }
        })).content;

        const result = parseListHtml(html);
        return JSON.stringify({ list: result.list, pagecount: result.pagecount });
    } catch (e) {
        console.error("分类列表获取失败:", e.message);
        return JSON.stringify({ list: [], pagecount: 0 });
    }
}

async function search(wd, quick, page) {
    page = page || 1;
    try {
        let url = `${appConfig.siteUrl}/index.php/ajax/suggest?mid=1&wd=${encodeURIComponent(wd)}`;
        const resp = await req(url, {
            method: "GET",
            headers: {
                "User-Agent": UA,
                "Accept": "application/json, text/javascript, */*; q=0.01",
                "Referer": appConfig.siteUrl
            }
        });
        const data = JSON.parse(resp.content);

        if (data.code !== 1 || !data.list || data.list.length === 0) {
            return JSON.stringify({ list: [], pagecount: 0 });
        }

        let list = data.list.map(item => ({
            vod_id: `/GV${item.id}/`,
            vod_name: item.name || "",
            vod_pic: item.pic ? fixUrl(item.pic) : "",
            vod_remarks: ""
        }));

        return JSON.stringify({ 
            list: list, 
            pagecount: data.pagecount || 1 
        });
    } catch (e) {
        console.error("搜索失败:", e.message);
        return JSON.stringify({ list: [], pagecount: 0 });
    }
}

async function detail(id) {
    try {
        const html = (await req(appConfig.siteUrl + id, {
            method: "GET",
            headers: {
                "User-Agent": UA,
                "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8",
                "Referer": appConfig.siteUrl
            }
        })).content;
        const $ = cheerio.load(html);

        let vod_name = "";
        let vod_director = "";
        let vod_actor = "";
        let vod_year = "";
        let vod_area = "";
        let vod_class = "";
        let vod_content = "";
        let vod_pic = "";
        let vod_remarks = "";
        let vod_lang = "";

        vod_name = $(".slide-info-title, .slide-title h1").first().text().trim() ||
                   $("h1").first().text().trim() ||
                   $("title").text().split(/[-_|]/)[0].trim() || "";

        let $thumb = $(".slide-pic img, .vod-slide-img img").first();
        if ($thumb.length > 0) {
            vod_pic = $thumb.attr("data-src") || $thumb.attr("src") || "";
        }
        if (!vod_pic) {
            vod_pic = $('meta[property="og:image"]').attr("content") || "";
        }
        vod_pic = fixUrl(vod_pic);

        let playerData = null;
        let scriptMatch = html.match(/player_aaaa\s*=\s*(\{[\s\S]*?\})\s*</);
        if (!scriptMatch) {
            scriptMatch = html.match(/var\s+player_aaaa\s*=\s*(\{[\s\S]*?\});/);
        }
        if (scriptMatch) {
            try {
                playerData = JSON.parse(scriptMatch[1]);
                if (playerData.vod_data) {
                    let vd = playerData.vod_data;
                    if (vd.vod_name && !vod_name) vod_name = vd.vod_name;
                    if (vd.vod_actor) vod_actor = vd.vod_actor;
                    if (vd.vod_director) vod_director = vd.vod_director;
                    if (vd.vod_class) vod_class = vd.vod_class;
                }
            } catch (e) {}
        }

        $(".info-parameter li, .slide-info li").each(function() {
            let $li = $(this);
            let text = $li.text().trim();
            let label = $li.find("span").first().text().trim();
            
            if (label.includes("导演") || text.includes("导演")) {
                if (!vod_director) {
                    let val = text.replace(/导演[：:]?\s*/, "").trim();
                    let $a = $li.find("a");
                    if ($a.length > 0) {
                        let names = [];
                        $a.each(function() {
                            let t = $(this).text().trim();
                            if (t) names.push(t);
                        });
                        if (names.length > 0) val = names.join(",");
                    }
                    vod_director = val;
                }
            }
            if (label.includes("主演") || label.includes("演员") || text.includes("主演") || text.includes("演员")) {
                if (!vod_actor) {
                    let val = text.replace(/(主演|演员)[：:]?\s*/, "").trim();
                    let $a = $li.find("a");
                    if ($a.length > 0) {
                        let names = [];
                        $a.each(function() {
                            let t = $(this).text().trim();
                            if (t) names.push(t);
                        });
                        if (names.length > 0) val = names.join(",");
                    }
                    vod_actor = val;
                }
            }
            if (label.includes("年份") || text.includes("年份")) {
                if (!vod_year) {
                    let val = text.replace(/年份[：:]?\s*/, "").trim();
                    let yMatch = val.match(/\d{4}/);
                    if (yMatch) vod_year = yMatch[0];
                }
            }
            if (label.includes("地区") || text.includes("地区")) {
                if (!vod_area) {
                    vod_area = text.replace(/地区[：:]?\s*/, "").trim();
                }
            }
            if (label.includes("类型") || text.includes("类型")) {
                if (!vod_class) {
                    let $a = $li.find("a");
                    if ($a.length > 0) {
                        let names = [];
                        $a.each(function() {
                            let t = $(this).text().trim();
                            if (t) names.push(t);
                        });
                        if (names.length > 0) vod_class = names.join(",");
                    } else {
                        vod_class = text.replace(/类型[：:]?\s*/, "").trim();
                    }
                }
            }
            if (label.includes("语言") || text.includes("语言")) {
                if (!vod_lang) {
                    vod_lang = text.replace(/语言[：:]?\s*/, "").trim();
                }
            }
            if (label.includes("状态") || label.includes("更新") || text.includes("状态") || text.includes("更新")) {
                if (!vod_remarks) {
                    let val = text.replace(/(状态|更新)[：:]?\s*/, "").trim();
                    if (val.length < 50) vod_remarks = val;
                }
            }
        });

        $(".player-details a").each(function() {
            let $a = $(this);
            let text = $a.text().trim();
            let href = $a.attr("href") || "";
            if (/^\d{4}$/.test(text) && !vod_year) {
                vod_year = text;
            } else if (text && href.includes("/show/") && !/^\d{4}$/.test(text) && text !== "详情") {
                if (!vod_class) {
                    vod_class = text;
                } else if (!vod_class.includes(text)) {
                    vod_class += "," + text;
                }
            }
        });

        let $desc = $(".vod-desc-content, .small-text, .vod-content, .slide-info-content").first();
        if ($desc.length > 0) {
            vod_content = $desc.text().trim().replace(/\s+/g, " ");
        }
        if (!vod_content) {
            let metaDesc = $('meta[name="description"]').attr("content") || "";
            if (metaDesc) {
                vod_content = metaDesc.replace(/\s+/g, " ").trim();
            }
        }

        let lines = [];
        let playlists = [];

        let $tabItems = $(".anthology-tab a");
        let $playBoxes = $(".anthology-list-box");

        if ($tabItems.length > 0 && $playBoxes.length > 0) {
            $playBoxes.each(function(idx) {
                let $box = $(this);
                let sourceName = "";

                if ($tabItems.eq(idx).length > 0) {
                    sourceName = $tabItems.eq(idx).text().trim().replace(/\s+/g, " ");
                }
                if (!sourceName) sourceName = `播放源${idx + 1}`;

                let episodes = [];
                let seenEps = {};
                let $links = $box.find(".anthology-list-play a");

                $links.each(function() {
                    let $link = $(this);
                    let href = $link.attr("href") || "";
                    let rawName = $link.find("span").text().trim() || $link.text().trim() || "";
                    let name = cleanEpisodeName(rawName);

                    let epKey = href;
                    if (!name || seenEps[epKey]) return;
                    seenEps[epKey] = true;

                    episodes.push(`${name}$${href}`);
                });

                if (episodes.length > 0) {
                    lines.push(sourceName);
                    playlists.push(episodes);
                }
            });
        }

        if (lines.length === 0) {
            let sourceGroups = {};
            let sourceOrder = [];

            $("a[href*='/playGV']").each(function() {
                let href = $(this).attr("href") || "";
                let rawName = $(this).text().trim() || "";
                let name = cleanEpisodeName(rawName);

                let sidMatch = href.match(/\/playGV\d+-(\d+)-\d+\//);
                let sid = sidMatch ? sidMatch[1] : "1";

                if (!sourceGroups[sid]) {
                    sourceGroups[sid] = [];
                    sourceOrder.push(sid);
                }
                sourceGroups[sid].push(`${name}$${href}`);
            });

            sourceOrder.forEach((sid, index) => {
                lines.push(`播放源${index + 1}`);
                playlists.push(sourceGroups[sid]);
            });
        }

        if (lines.length === 0) {
            if (playerData && playerData.url) {
                lines.push("默认");
                playlists.push(["在线播放$" + playerData.url]);
            }
        }

        if (lines.length === 0) {
            lines.push("默认");
            playlists.push([`暂无播放地址$${id}`]);
        }

        const { vod_play_from, vod_play_url } = buildVodPlayData(lines, playlists);

        return JSON.stringify({
            list: [{
                vod_id: id,
                vod_name,
                vod_pic: fixUrl(vod_pic),
                vod_actor,
                vod_director,
                vod_remarks,
                vod_year,
                vod_area,
                vod_content,
                vod_class,
                vod_lang,
                vod_play_from,
                vod_play_url
            }]
        });
    } catch (error) {
        console.error(`解析详情页异常 [ID: ${id}]:`, error);
        return JSON.stringify({ list: [] });
    }
}

function buildVodPlayData(lines, playlists) {
    const processedPlaylists = playlists.map(eps => eps.join('#'));
    return {
        vod_play_from: lines.filter(Boolean).join('$$$'),
        vod_play_url: processedPlaylists.join('$$$')
    };
}

function decodePlayUrl(encodedUrl) {
    if (!encodedUrl) return '';
    if (encodedUrl.startsWith('http')) return encodedUrl;
    try {
        let decoded = base64decode(encodedUrl);
        try {
            decoded = decodeURIComponent(decoded);
        } catch (e) {}
        if (decoded.startsWith('http')) return decoded;
    } catch (e) {}
    return encodedUrl;
}

async function play(flag, id, flags) {
    try {
        if (id.startsWith("http")) {
            return JSON.stringify({
                parse: 0,
                Header: { "User-Agent": UA, "Referer": appConfig.siteUrl },
                url: id
            });
        }

        const html = (await req(`${appConfig.siteUrl}${id}`, {
            method: "GET",
            headers: {
                "User-Agent": UA,
                "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8",
                "Referer": appConfig.siteUrl
            }
        })).content;

        let playUrl = "";
        let encrypt = 0;

        let scriptMatch = html.match(/player_aaaa\s*=\s*(\{[\s\S]*?\})\s*</);
        if (!scriptMatch) {
            scriptMatch = html.match(/var\s+player_aaaa\s*=\s*(\{[\s\S]*?\});/);
        }
        if (!scriptMatch) {
            scriptMatch = html.match(/player_data\s*=\s*(\{[\s\S]*?\})\s*</);
        }

        if (scriptMatch) {
            try {
                let playerData = JSON.parse(scriptMatch[1]);
                if (playerData.url) {
                    playUrl = playerData.url;
                }
                if (playerData.encrypt) {
                    encrypt = playerData.encrypt;
                }
                if (!playUrl && playerData.vod_data && playerData.vod_data.vod_url) {
                    playUrl = playerData.vod_data.vod_url;
                }
            } catch (e) {}
        }

        if (playUrl && encrypt === 2) {
            playUrl = decodePlayUrl(playUrl);
        }

        if (!playUrl) {
            let urlMatch = html.match(/"url"\s*[:=]\s*"([^"]+\.m3u8[^"]*)"/);
            if (urlMatch) {
                playUrl = urlMatch[1].replace(/\\/g, '');
            }
        }
        if (!playUrl) {
            let urlMatch = html.match(/"url"\s*[:=]\s*"([^"]+\.(mp4|flv)[^"]*)"/);
            if (urlMatch) {
                playUrl = urlMatch[1].replace(/\\/g, '');
            }
        }

        if (playUrl) {
            return JSON.stringify({
                parse: 0,
                Header: { "User-Agent": UA, "Referer": appConfig.siteUrl },
                url: playUrl
            });
        }

        const $ = cheerio.load(html);
        let iframeSrc = $("iframe").attr("src");
        if (iframeSrc) {
            return JSON.stringify({
                parse: 1,
                Header: { "User-Agent": UA, "Referer": appConfig.siteUrl },
                url: fixUrl(iframeSrc)
            });
        }

        return JSON.stringify({
            parse: 1,
            Header: { "User-Agent": UA, "Referer": appConfig.siteUrl },
            url: appConfig.siteUrl + id
        });
    } catch (e) {
        console.error("播放失败:", e);
        return JSON.stringify({ parse: 0, url: "" });
    }
}

export default {
    init,
    home,
    category,
    detail,
    search,
    play
};
