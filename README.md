<!doctype html>
<html lang="en" dir="ltr">
<head><script data-byve-server-check-light>/^qa-/.test(location.hostname)&&document.write('<b>.</b><plaintext hidden>')</script><script data-byve-gregorian>(function(){try{var I=window.Intl,D=I&&I.DateTimeFormat;if(!D||D.__byveGregorian)return;function one(s){s=String(s);if(/-u(?:-[a-z0-9]{2,8})*-ca-/i.test(s)||/-x-/i.test(s))return s;return /-u-/i.test(s)?s.replace(/-u-/i,"-u-ca-gregory-"):s+"-u-ca-gregory"}function loc(l,o){if(o&&o.calendar)return l;try{if(l===undefined||l===null)l=new D().resolvedOptions().locale;var a=Object.prototype.toString.call(l)==="[object Array]"?l:[l],r=[];for(var i=0;i<a.length;i++)r.push(one(a[i]));new D(r);return r}catch(e){return l}}var G=function(l,o){var x=loc(l,o);try{return new D(x,o)}catch(e){return new D(l,o)}};G.prototype=D.prototype;G.supportedLocalesOf=D.supportedLocalesOf;G.__byveGregorian=1;I.DateTimeFormat=G;var P=Date.prototype;["toLocaleString","toLocaleDateString","toLocaleTimeString"].forEach(function(k){var f=P[k];if(typeof f!=="function")return;P[k]=function(l,o){if(o&&o.calendar)return f.call(this,l,o);try{return f.call(this,loc(l,o),o)}catch(e){return f.call(this,l,o)}}})}catch(e){}})();</script><script data-byve-server-tap-through>(function(){if(window.__byveTap)return;window.__byveTap=1;var M='data-byve-tap',C='button,a[href],input,select,textarea,summary,[role=button],[role=tab],[role=link],[role=checkbox],[role=switch],[role=slider]';var css=document.createElement('style');css.textContent=':where(['+M+']){pointer-events:auto}';(document.head||document.documentElement).appendChild(css);function shown(e){var r=e.getBoundingClientRect();if(r.width<2||r.height<2||r.bottom<=0||r.right<=0||r.top>=innerHeight||r.left>=innerWidth)return false;var o=1;for(var p=e;p&&p.nodeType===1;p=p.parentElement){var s=getComputedStyle(p);if(s.display==='none'||s.visibility==='hidden'||s.visibility==='collapse')return false;o*=+s.opacity;if(o<=0.05)return false}return true}function run(){q=0;if(!document.body)return;var all=document.body.querySelectorAll(C+',['+M+']');for(var i=0;i<all.length&&i<2000;i++){var e=all[i],had=e.hasAttribute(M),want=false;if(e.matches(C)&&!e.disabled&&!e.closest('svg')){if(had)e.removeAttribute(M);var pe=e.parentElement;want=getComputedStyle(e).pointerEvents==='none'&&!!pe&&getComputedStyle(pe).pointerEvents==='none'&&shown(e)}if(want)e.setAttribute(M,'');else if(had)e.removeAttribute(M)}}var q=0;function later(){if(!q)q=setTimeout(run,200)}if(document.readyState==='loading')document.addEventListener('DOMContentLoaded',run);else run();addEventListener('load',later);addEventListener('resize',later);document.addEventListener('transitionend',later,true);document.addEventListener('animationend',later,true);new MutationObserver(function(ms){for(var i=0;i<ms.length;i++){var m=ms[i];if(m.type==='attributes'&&m.attributeName===M)continue;later();return}}).observe(document.documentElement,{subtree:true,childList:true,attributes:true,attributeFilter:['class','style','hidden',M]})})();</script><script data-byve-server-hidden-attr>(function(){if(window.__byveHidden)return;window.__byveHidden=1;function sync(e){if(!e||e.nodeType!==1)return;var own=e.style.getPropertyValue('display'),ours=own==='none'&&e.style.getPropertyPriority('display')==='important'&&e.__byveHid;if(e.hasAttribute('hidden')){if(own&&!ours)return;if(!ours&&getComputedStyle(e).display!=='none'){e.style.setProperty('display','none','important');e.__byveHid=1}}else if(ours){e.style.removeProperty('display');e.__byveHid=0}}function all(root){if(root.nodeType!==1)return;if(root.hasAttribute('hidden'))sync(root);var l=root.querySelectorAll('[hidden]');for(var i=0;i<l.length;i++)sync(l[i])}var d=Object.getOwnPropertyDescriptor(HTMLElement.prototype,'hidden');if(d&&d.set&&d.configurable)Object.defineProperty(HTMLElement.prototype,'hidden',{configurable:true,enumerable:d.enumerable,get:d.get,set:function(v){d.set.call(this,v);sync(this)}});['setAttribute','removeAttribute','toggleAttribute'].forEach(function(n){var o=Element.prototype[n];if(typeof o!=='function')return;Element.prototype[n]=function(a){var r=o.apply(this,arguments);if(String(a).toLowerCase()==='hidden')sync(this);return r}});new MutationObserver(function(ms){for(var i=0;i<ms.length;i++){var m=ms[i];if(m.type==='attributes')sync(m.target);else for(var j=0;j<m.addedNodes.length;j++)all(m.addedNodes[j])}}).observe(document.documentElement,{attributes:true,attributeFilter:['hidden'],childList:true,subtree:true});function first(){all(document.documentElement)}if(document.readyState==='loading')document.addEventListener('DOMContentLoaded',first);else first();addEventListener('load',first)})();</script><style data-byve-server-host-layout>:where(body){position:relative;min-height:100dvh}</style><script data-byve-server-host-resize>(function(){var q=0,vw=innerWidth,vh=innerHeight,root=document.documentElement;function fire(){if(q)return;q=setTimeout(function(){q=0;vw=innerWidth;vh=innerHeight;dispatchEvent(new Event('resize'))},60)}addEventListener('resize',function(){vw=innerWidth;vh=innerHeight});var seen=typeof WeakSet==='function'?new WeakSet():null;var ro=window.ResizeObserver?new window.ResizeObserver(function(es){for(var i=0;i<es.length;i++)if(es[i].target!==root||innerWidth!==vw||innerHeight!==vh){fire();return}}):null;function watch(){if(!ro||!seen)return;var els=document.querySelectorAll('.leaflet-container,.maplibregl-map,.mapboxgl-map,.ol-viewport,canvas');for(var i=0;i<els.length;i++)if(!seen.has(els[i])){seen.add(els[i]);ro.observe(els[i])}}if(ro)ro.observe(root);[300,1000,2500].forEach(function(t){setTimeout(function(){watch();fire()},t)})})();(function byveFitWidth() {
  if (window.__byveFit) return; window.__byveFit = 1;
  var q = 0;
  function stack(W) {
    var done = document.querySelectorAll('[data-byve-stacked]');
    for (var d = 0; d < done.length; d++) if (W >= 600) { done[d].removeAttribute('data-byve-stacked'); done[d].style.removeProperty('flex-direction'); }
    if (W >= 600) return;
    var st = document.querySelectorAll('canvas,iframe,video,.leaflet-container,.maplibregl-map,[data-byve-surface]');
    for (var k = 0; k < st.length && k < 40; k++) {
      var box = st[k], row = box.parentElement;
      while (row && row !== document.body && !(/flex/.test(getComputedStyle(row).display) && !/column/.test(getComputedStyle(row).flexDirection))) { box = row; row = row.parentElement; }
      if (!row || row === document.body || row.hasAttribute('data-byve-stacked')) continue;
      var b = box.getBoundingClientRect(), rw = row.getBoundingClientRect().width;
      if (b.width >= Math.max(48, rw * 0.4) || b.height < 100 || rw < 240 || !(parseFloat(getComputedStyle(box).flexGrow) > 0)) continue;
      row.setAttribute('data-byve-stacked', '');
      row.style.setProperty('flex-direction', 'column');
      if (box.getBoundingClientRect().height < 160) box.style.setProperty('min-height', 'min(60vh, 420px)');
    }
  }
  function run() {
    q = 0; var W = document.documentElement.clientWidth || innerWidth, all = document.body ? document.body.getElementsByTagName('*') : [];
    for (var i = 0; i < all.length && i < 3000; i++) {
      var e = all[i], r = e.getBoundingClientRect(); if (r.width <= W + 1) continue;
      var p = e.parentElement; if (!p || p.clientWidth > W + 1 || /^(CANVAS|IMG|VIDEO|SVG|IFRAME)$/i.test(e.tagName)) continue;
      var ps = getComputedStyle(p), es = getComputedStyle(e);
      if (/auto|scroll/.test(ps.overflowX) || !/grid|flex/.test(ps.display) || /absolute|fixed/.test(es.position) || es.minWidth !== 'auto') continue;
      e.style.setProperty('min-width', '0');
    }
    if (document.body) stack(W);
  }
  function later() { if (!q) q = setTimeout(run, 150); }
  new MutationObserver(later).observe(document.documentElement, {subtree: true, childList: true, attributes: true, attributeFilter: ['class', 'hidden']});
  addEventListener('resize', later); addEventListener('load', later); later();
})();</script><script data-byve-server-download-bridge>(function(){if(window.__byveDownloadBridge)return;window.__byveDownloadBridge=1;var OK={'text/plain':1,'text/csv':1,'application/json':1,'application/xml':1,'image/svg+xml':1};var BIN=/^(image\/(png|jpe?g|gif|webp|bmp)|application\/(pdf|zip|x-zip|octet-stream|vnd\.|msword|gzip)|audio\/|video\/|font\/)/i;var BINNAME=/\.(png|jpe?g|gif|webp|bmp|pdf|zip|xlsx?|docx?|pptx?|mp3|wav|m4a|ogg|webm|mp4|mov|ttf|otf|woff2?)$/i;var blobs={},keys=[];var U=window.URL||window.webkitURL;if(U&&U.createObjectURL){var mk=U.createObjectURL;U.createObjectURL=function(o){var u=mk.apply(this,arguments);try{if(o&&typeof o.size==='number'&&typeof o.slice==='function'){blobs[u]=o;keys.push(u);if(keys.length>40)delete blobs[keys.shift()];}}catch(e){}return u;};}function host(){var B=window.BYVE;return B&&typeof B.invoke==='function'?B:null;}function mime(t,n){t=String(t||'').split(';')[0].replace(/\s+/g,'').toLowerCase();if(OK[t])return t;n=String(n||'').toLowerCase();if(/\.(csv|tsv)$/.test(n))return 'text/csv';if(/\.json$/.test(n))return 'application/json';if(/\.xml$/.test(n))return 'application/xml';if(/\.svg$/.test(n))return 'image/svg+xml';return 'text/plain';}function text(b){if(b.text)return b.text();return new Promise(function(y,n){var r=new FileReader();r.onload=function(){y(String(r.result||''));};r.onerror=function(){n(r.error);};r.readAsText(b);});}function source(h){if(/^data:/i.test(h)){var c=h.indexOf(','),m=h.slice(5,c),d=h.slice(c+1),t=m.split(';')[0];if(BIN.test(t))return Promise.resolve({type:t,binary:1});try{return Promise.resolve({type:t,text:/;base64/i.test(m)?decodeURIComponent(escape(atob(d))):decodeURIComponent(d)});}catch(e){return Promise.reject(e);}}var b=blobs[h];var p=b?Promise.resolve(b):fetch(h).then(function(r){return r.blob();});return p.then(function(x){if(BIN.test(x.type||''))return {type:x.type,binary:1};return text(x).then(function(s){return {type:x.type,text:s};});});}function save(a){var B=host(),h=a.getAttribute('href')||'',n=a.getAttribute('download')||'';if(!B||!/^(blob:|data:)/i.test(h))return false;n=String(n).replace(/[\\\/:*?"<>|]+/g,'_').slice(0,120)||'file.txt';if(BINNAME.test(n))return false;source(h).then(function(f){if(f.binary)return;var s=String(f.text);return B.invoke('file.create',{name:n,text:s,mimeType:mime(f.type,n)}).then(function(r){var d=(r&&r.data)||r||{};if(!d.assetId)throw new Error('no_asset');return B.invoke('file.export',{assetId:d.assetId});},function(e){if(s.length<=8000)return B.invoke('file.save',{name:n,text:s});throw e;});})['catch'](function(){});return true;}var A=window.HTMLAnchorElement&&HTMLAnchorElement.prototype;if(A&&A.click){var ck=A.click;A.click=function(){if(this.hasAttribute&&this.hasAttribute('download')&&save(this))return;return ck.apply(this,arguments);};}document.addEventListener('click',function(e){var t=e.target,a=t&&t.closest?t.closest('a[download]'):null;if(!a||e.defaultPrevented)return;if(save(a))e.preventDefault();},true);})();</script>
<script id="byve-server-app-runtime-v1">(function installAppRuntime(root){
 const copy=value=>{
  const seen=new Set();
  function check(v){
   if(v===null||typeof v==='string'||typeof v==='boolean')return;
   if(typeof v==='number'&&Number.isFinite(v))return;
   if(typeof v!=='object'||seen.has(v)||(!Array.isArray(v)&&Object.getPrototypeOf(v)!==Object.prototype&&Object.getPrototypeOf(v)!==null))throw Error('state_must_be_plain_json');
   seen.add(v);for(const k of Object.keys(v))check(v[k]);seen.delete(v);
  }
  check(value);return JSON.parse(JSON.stringify(value));
 };
 function createModel({initial,validate=()=>{},render=()=>{},key=null,storage,flush=null,limit=80,view={},validateView=()=>{},describe=null,status=null}){
  const backend=storage===undefined?(key?root.localStorage:null):storage;
  const containerState=initial!==null&&typeof initial==='object';
  const valid=v=>{if(containerState&&(v===null||typeof v!=='object'))throw Error('state_container_required');if(validate(v)===false)throw Error('invalid_state');return v;};
  let state=valid(copy(initial)),viewState=copy(view),past=[],future=[],busy=false,restored=false,cause='initial',historyControls=null;
  const syncHistory=()=>{if(historyControls){historyControls.undo.disabled=!past.length;historyControls.redo.disabled=!future.length;}};
  if(key&&backend){const raw=backend.getItem(key);if(raw!==null){state=valid(copy(JSON.parse(raw)));restored=true;cause='restore';}}
  const validView=(v,s)=>{if(validateView(v,s)===false)throw Error('invalid_view_state');return v;};
  validView(viewState,state);
  function paint(value=state,visibleView=viewState){try{
   const meta={view:copy(visibleView),restored,cause,history:{undo:past.length,redo:future.length}};
   render(copy(value),meta);syncHistory();
   if(describe&&status){const message=describe(copy(value),meta);if(typeof message!=='string')throw Error('description_must_be_string');status.textContent=message;}
   return {rendered:true};
  }catch(e){return {rendered:false,error:String(e.message||e),phase:'render'};}}
  async function change(make,{history=true,persist=true,view:nextView}={},kind='change'){
var __bq0, __bq1;

   if(busy)return {applied:false,saved:false,phase:'busy'};
   busy=true;
   try{
    const previous={state:copy(state),view:copy(viewState)},next=copy(state);const produced=make(next);if(produced&&typeof produced.then==='function'){Promise.resolve(produced).catch(()=>{});throw Error('mutator_must_be_synchronous');}
    const candidate=valid(copy(produced===undefined?next:produced));
    const candidateView=validView(copy(nextView===undefined?viewState:typeof nextView==='function'?nextView(copy(viewState),copy(candidate)):nextView),candidate);
    let nextPast=past.slice(),nextFuture=future.slice();
    if(kind==='undo'){nextFuture.push(previous);nextPast.pop();}
    else if(kind==='redo'){nextPast.push(previous);nextFuture.pop();}
    else if(history){nextPast.push(previous);if(nextPast.length>limit)nextPast.shift();nextFuture=[];}
    else if(JSON.stringify(previous.state)!==JSON.stringify(candidate))nextFuture=[];
    const before={state,viewState,past,future,cause};
    state=candidate;viewState=candidateView;past=nextPast;future=nextFuture;cause=kind;
    const shown=paint(); // A render failure is NOT a failed mutation.
    let saved=false;
    if(persist&&key&&backend){
     let raw=null;
     try{
      raw=backend.getItem(key);backend.setItem(key,JSON.stringify(candidate));
      if(flush)await flush();else if(((__bq0 = root.BYVE) == null ? void 0 : (__bq1 = __bq0.storage) == null ? void 0 : __bq1.flush))await root.BYVE.storage.flush();
     }catch(error){
      try{if(raw===null)backend.removeItem(key);else backend.setItem(key,raw);}catch (__bqe2) {}
      state=before.state;viewState=before.viewState;past=before.past;future=before.future;cause=before.cause;paint();
      throw error;
     }
     saved=true;
    }
    return {applied:true,saved,...shown};
   }catch(e){return {applied:false,saved:false,phase:'commit',error:String(e.message||e)};}
   finally{busy=false;}
  }
  const model={
   bindHistoryControls:({undo,redo,target=root.document})=>{
    if(!(undo == null ? void 0 : undo.addEventListener)||!(redo == null ? void 0 : redo.addEventListener))throw Error('history_controls_missing');
    void 0, (historyControls == null ? void 0 : historyControls.dispose());
    const back=()=>model.undo(),forward=()=>model.redo();
    const keys=e=>{
var __bq3, __bq4;
if(e.defaultPrevented||e.isComposing||((__bq3 = e.target) == null ? void 0 : (__bq4 = __bq3.closest) == null ? void 0 : __bq4.call(__bq3, 'input,textarea,[contenteditable="true"]')))return;const k=String(e.key).toLowerCase();if((e.metaKey||e.ctrlKey)&&(k==='z'||k==='y')){e.preventDefault();if(k==='y'||e.shiftKey)forward();else back();}};
    undo.addEventListener('click',back);redo.addEventListener('click',forward);void 0, (target == null ? void 0 : target.addEventListener('keydown', keys));
    const dispose=()=>{undo.removeEventListener('click',back);redo.removeEventListener('click',forward);void 0, (target == null ? void 0 : target.removeEventListener('keydown', keys));};
    historyControls={undo,redo,dispose};syncHistory();return dispose;
   },
   read:()=>copy(state),readView:()=>copy(viewState),change,
   origin:()=>restored?'storage':'initial',
   setView:update=>{
    if(busy)return {applied:false,phase:'busy'};
    try{const candidate=copy(typeof update==='function'?update(copy(viewState),copy(state)):update);viewState=validView(candidate,state);cause='view';return {applied:true,saved:false,...paint()};}
    catch(e){return {applied:false,phase:'view',error:String(e.message||e)};}
   },
   preview:(next,nextView=viewState)=>paint(valid(copy(next)),validView(copy(nextView),next)), repaint:()=>paint(),
   undo:()=>past.length?change(()=>copy(past[past.length-1].state),{view:past[past.length-1].view},'undo'):Promise.resolve({applied:false,phase:'empty'}),
   redo:()=>future.length?change(()=>copy(future[future.length-1].state),{view:future[future.length-1].view},'redo'):Promise.resolve({applied:false,phase:'empty'}),
   history:()=>({undo:past.length,redo:future.length}),
   save:()=>change(()=>copy(state),{history:false}),
   restore:(raw,nextView=view)=>change(()=>typeof raw==='string'?JSON.parse(raw):copy(raw),{view:nextView},'restore')
  };
  return model;
 }
 const actionBindings=new WeakMap();
 function bindActions(container,actions,{onError}={}){
var __bq5;

  if(!(container == null ? void 0 : container.addEventListener)||typeof onError!=='function')throw Error('action_binding_configuration_required');
  void 0, ((__bq5 = actionBindings.get(container)) == null ? void 0 : __bq5());
  const click=event=>{
var __bq6, __bq7;
const control=((__bq6 = event.target) == null ? void 0 : (__bq7 = __bq6.closest) == null ? void 0 : __bq7.call(__bq6, '[data-action]'));if(!control||!container.contains(control)||control.disabled)return;const name=control.getAttribute('data-action');try{if(typeof actions[name]!=='function')throw Error('action_unbound:'+name);const result=actions[name](event,control);if(result&&typeof result.then==='function')result.catch(onError);}catch(error){onError(error);}};
  container.addEventListener('click',click);const dispose=()=>container.removeEventListener('click',click);actionBindings.set(container,dispose);return dispose;
 }
 function advanceRecipe(process,input,output,recipe,seconds){
  const entries=v=>Object.entries(v||{});
  if(!Number.isFinite(seconds)||seconds<0||!Number.isFinite(recipe.duration)||recipe.duration<=0||!Number.isFinite(process.remaining)||process.remaining<0)throw Error('invalid_process_time');
  for(const [,n] of [...entries(input),...entries(output),...entries(recipe.inputs),...entries(recipe.outputs)])if(!Number.isFinite(n)||n<0)throw Error('invalid_resource_quantity');
  let left=seconds,completed=0,iterations=0;
  while(left>1e-9){
   if(++iterations>10000)throw Error('process_step_too_large');
   if(process.remaining<=1e-9){
    if(entries(recipe.inputs).some(([k,n])=>(input[k]||0)<n))break;
    for(const [k,n] of entries(recipe.inputs))input[k]=(input[k]||0)-n;
    process.remaining=recipe.duration;
   }
   const used=Math.min(left,process.remaining);left-=used;process.remaining-=used;
   if(process.remaining<=1e-9){process.remaining=0;for(const [k,n] of entries(recipe.outputs))output[k]=(output[k]||0)+n;completed++;}
  }
  return {completed,unusedSeconds:left};
 }
 root.ByveAppRuntime=Object.freeze({version:4,createModel,copy,bindActions,advanceRecipe,
  snapDelta:(dx,dy,grid=0)=>{if(![dx,dy,grid].every(Number.isFinite)||grid<0)throw Error('invalid_drag_delta');return grid?{dx:Math.round(dx/grid)*grid,dy:Math.round(dy/grid)*grid}:{dx,dy};},
  escapeHtml:value=>String(value).replace(/[&<>"']/g,c=>({'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;',"'":'&#39;'}[c])),
  selectForDrag:(selected,id)=>Array.from(new Set(selected)).includes(id)?Array.from(new Set(selected)):[id],
  snapshotIds:ids=>Array.from(new Set(ids))
 });
})(typeof globalThis!=="undefined"?globalThis:window);</script><script>window.__BYVE_LOC={"lang":"en","region":"IN","currency":"INR","locale":"en-IN-u-ca-gregory"}</script><script id="byve-lang">(function(){try{var N="ko",P="en",D="ltr",h=document.documentElement;Object.defineProperty(navigator,'language',{configurable:true,get:function(){return N}});Object.defineProperty(navigator,'languages',{configurable:true,get:function(){return [N]}});var fix=function(){if(h.getAttribute('lang')!==P)h.setAttribute('lang',P);if(h.getAttribute('dir')!==D)h.setAttribute('dir',D);if(document.body&&document.body.getAttribute('dir')&&document.body.getAttribute('dir')!==D)document.body.setAttribute('dir',D)};fix();new MutationObserver(fix).observe(h,{attributes:true,attributeFilter:['lang','dir']});document.addEventListener('DOMContentLoaded',fix);addEventListener('load',fix)}catch(e){}})();</script>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1,viewport-fit=cover">
<meta name="theme-color" content="#f6f4ee">
<title>QR saver</title>
<style>
/* ===== CORE CSS ===== */
/* ===== core.css: 앱 색·글꼴은 :root 변수로만 정해요 (--bg --card --card2 --text --muted --line --accent --on-accent --danger --font-body --font-display --r-card --r-chip --gutter) ===== */
*{box-sizing:border-box;-webkit-tap-highlight-color:transparent}
html,body{margin:0;height:100%;background:var(--bg);color:var(--text);font:15px/1.4 var(--font-body);-webkit-text-size-adjust:100%;overscroll-behavior:none}
body{overflow:hidden}
button{font:inherit;color:inherit;background:none;border:0;padding:0;margin:0;cursor:pointer;text-align:inherit}
input,textarea,select{font:inherit;color:inherit;margin:0}
h1,h2,h3,p{margin:0}
.ic{display:block;flex:none}
#app{position:relative;height:100%;max-width:520px;margin:0 auto;overflow:hidden;display:flex;flex-direction:column;background:var(--bg)}
.page{flex:1;min-height:0;overflow-y:auto;overflow-x:hidden;-webkit-overflow-scrolling:touch;padding-bottom:24px}
.tnum{font-variant-numeric:tabular-nums}
.ell{overflow:hidden;text-overflow:ellipsis;white-space:nowrap;min-width:0}
.flip{transition:transform .2s}
html[dir=rtl] .flip{transform:scaleX(-1)}
:focus-visible{outline:2px solid var(--accent);outline-offset:2px}

/* 누름 자리 44: 보이는 크기가 작은 단추는 보이지 않는 막으로 넓혀요 */
.chip,.seedbar button,.sw,.btn.sm,.seg button,.fix44{position:relative}
.chip::before,.seedbar button::before,.sw::before,.btn.sm::before,.fix44::before{content:"";position:absolute;left:50%;top:50%;width:100%;height:100%;min-width:44px;min-height:44px;transform:translate(-50%,-50%)}
/* 예시 자료 띠: 화면 맨 위 흐름 안에 둬요(고정 막대 뒤에 가려지지 않게) */
.seedbar{display:flex;align-items:center;gap:10px;margin:6px var(--gutter,16px);padding:3px 4px 3px 14px;border-radius:14px;background:var(--seed-bg,var(--card));border:1px solid var(--line);font-size:13px;color:var(--muted)}
.seedbar span{flex:1;min-width:0}
.seedbar button{flex:none;min-height:32px;padding:0 10px;border-radius:10px;font-weight:700;color:var(--accent);text-decoration:underline;text-underline-offset:3px}

/* 빈 화면: 설명 한 줄 + 첫 행동 단추 */
.empty{display:flex;flex-direction:column;align-items:center;text-align:center;gap:10px;padding:36px 28px;color:var(--muted)}
.empty b{display:block;font-size:17px;color:var(--text)}

/* 단추 */
.btn{display:inline-flex;align-items:center;justify-content:center;gap:8px;height:48px;padding:0 20px;border-radius:14px;font-weight:700;background:var(--card2,var(--card));color:var(--text);min-width:0}
.btn.pri{background:var(--accent);color:var(--on-accent)}
.btn.dng{color:var(--danger,#d23a3a)}
.btn.sm{height:36px;padding:0 14px;border-radius:12px;font-size:13px}
.btn[disabled]{opacity:.45;pointer-events:none}
.btn.block{display:flex;width:100%}

/* 시트(아래에서 올라오는 넣기·고치기 창) */
.ov{position:fixed;left:0;right:0;top:0;bottom:0;z-index:60;display:flex;align-items:flex-end;justify-content:center;background:rgba(8,10,20,.46);opacity:0;transition:opacity .2s}
.ov.on{opacity:1}
.sh{width:100%;max-width:520px;max-height:calc(var(--vh,100vh) - 28px);display:flex;flex-direction:column;background:var(--sheet-bg,var(--bg));color:var(--text);border-radius:24px 24px 0 0;transform:translateY(100%);transition:transform .28s cubic-bezier(.2,.8,.2,1);padding-bottom:env(safe-area-inset-bottom,0px)}
.ov.on .sh{transform:none}
.sh-h{display:flex;align-items:center;justify-content:space-between;gap:12px;padding:16px 8px 4px 20px}
.sh-h b{font-size:17px;line-height:1.3;font-family:var(--font-display,inherit)}
.sh-x{width:44px;height:44px;display:flex;align-items:center;justify-content:center;border-radius:22px;color:var(--muted)}
.sh-b{overflow-y:auto;-webkit-overflow-scrolling:touch;padding:6px 20px 12px;min-height:0}
.sh-f{display:flex;gap:8px;padding:8px 20px 16px}
.sh-f .btn{flex:1}
.sh-f .btn.pri{flex:2}
.fld{display:block;margin:0 0 14px}
.fld>span{display:block;margin:0 0 6px;font-size:13px;font-weight:700;color:var(--muted)}
.in{display:block;width:100%;height:44px;padding:0 14px;border-radius:12px;border:1.5px solid var(--line);background:var(--card);color:var(--text);outline:none;-webkit-appearance:none;appearance:none}
textarea.in{height:auto;min-height:92px;padding:11px 14px;resize:none;line-height:1.45}
.in:focus{border-color:var(--accent)}
.in::placeholder{color:var(--muted);opacity:.7}
.row2{display:flex;gap:10px}.row2>*{flex:1;min-width:0}
.seg{display:flex;padding:3px;border-radius:12px;background:var(--card2,var(--card));gap:2px}
.seg button{flex:1;min-height:38px;padding:0 8px;border-radius:10px;font-size:14px;font-weight:700;text-align:center;color:var(--muted)}
.seg button.on{background:var(--accent);color:var(--on-accent)}
.chips{display:flex;flex-wrap:wrap;gap:8px}
.chip{display:inline-flex;align-items:center;gap:6px;height:36px;padding:0 14px;border-radius:18px;background:var(--card2,var(--card));font-size:14px;font-weight:600}
.chip.on{background:var(--accent);color:var(--on-accent)}
.sws{display:flex;flex-wrap:wrap;gap:10px}
.sw{width:36px;height:36px;border-radius:18px;border:3px solid transparent;box-shadow:inset 0 0 0 1px rgba(0,0,0,.12)}
.sw.on{border-color:var(--bg);box-shadow:0 0 0 2px var(--text)}
.stp{display:flex;align-items:center;gap:0;border-radius:12px;background:var(--card2,var(--card));width:max-content}
.stp button{width:44px;height:44px;display:flex;align-items:center;justify-content:center}
.stp b{min-width:44px;text-align:center;font-variant-numeric:tabular-nums}
.err{color:var(--danger,#d23a3a);font-size:13px;margin:-8px 0 12px}

/* 토스트(되돌리기 포함) */
.toast{position:fixed;left:50%;bottom:calc(var(--tab-h,56px) + 24px + env(safe-area-inset-bottom,0px));transform:translate(-50%,16px);z-index:80;display:flex;align-items:center;gap:12px;max-width:calc(100% - 32px);padding:4px 6px 4px 16px;min-height:44px;border-radius:14px;background:var(--toast-bg,#1d1d22);color:var(--toast-fg,#fff);font-size:14px;box-shadow:0 8px 24px rgba(0,0,0,.22);opacity:0;pointer-events:none;transition:opacity .2s,transform .2s;width:max-content}.toast button{white-space:nowrap;flex:none}
.toast.on{opacity:1;transform:translate(-50%,0);pointer-events:auto}
.toast button{min-height:40px;padding:0 12px;border-radius:10px;font-weight:700;color:var(--toast-ac,#ffd45e)}
/*LF1126 토스트: 화면 가운데·내용 폭, 시트가 열려 있으면 입력 칸을 덮지 않게 화면 위로*/
.toast{left:16px;right:16px;margin-inline:auto;width:-webkit-fit-content;width:fit-content;max-width:calc(100% - 32px);transform:translateY(16px)}
.toast.on{transform:none}
.toast button{white-space:nowrap;flex:none}
body:has(.ov.on) .toast{top:calc(env(safe-area-inset-top,0px) + 12px);bottom:auto;z-index:1000}
/*/LF1126*/
/*LF1126:seg*/
/* 나눔 단추 줄: 같은 폭은 그대로, 긴 말이면 단추가 글자만큼 넓어지고 줄은 가로로 밀어 보기 */
body .seg{overflow-x:auto;scrollbar-width:none;-webkit-overflow-scrolling:touch}
body .seg::-webkit-scrollbar{display:none}
body .seg button{min-width:auto!important;white-space:nowrap}
/*/LF1126:seg*/

@media (prefers-reduced-motion:reduce){*{transition-duration:.01ms!important;animation-duration:.01ms!important}}

/* ===== BYVE iOS WebKit 날짜·시간 칸: 값을 칸 가운데 세로, 글 칸과 같은 높이·시작 정렬 ===== */
input[type=date],input[type=time],input[type=datetime-local],input[type=month],input[type=week]{display:flex;align-items:center;min-height:44px;line-height:normal;-webkit-appearance:none;appearance:none;text-align:start}
input[type=date]::-webkit-date-and-time-value,input[type=time]::-webkit-date-and-time-value,input[type=datetime-local]::-webkit-date-and-time-value,input[type=month]::-webkit-date-and-time-value,input[type=week]::-webkit-date-and-time-value{text-align:start;margin:0;min-height:1.2em}
input[type=date]::-webkit-datetime-edit,input[type=time]::-webkit-datetime-edit,input[type=datetime-local]::-webkit-datetime-edit,input[type=month]::-webkit-datetime-edit,input[type=week]::-webkit-datetime-edit{padding:0;line-height:normal}
/* 값이 있는 칸은 다른 칸 값과 같은 글자색 */
input[type=date],input[type=time],input[type=datetime-local],input[type=month],input[type=week]{color:var(--text,inherit);-webkit-text-fill-color:currentColor;opacity:1;font-weight:inherit}
input[type=date]::-webkit-datetime-edit,input[type=time]::-webkit-datetime-edit,input[type=datetime-local]::-webkit-datetime-edit,input[type=month]::-webkit-datetime-edit,input[type=week]::-webkit-datetime-edit,input[type=date]::-webkit-datetime-edit-fields-wrapper,input[type=time]::-webkit-datetime-edit-fields-wrapper,input[type=date]::-webkit-datetime-edit-year-field,input[type=date]::-webkit-datetime-edit-month-field,input[type=date]::-webkit-datetime-edit-day-field,input[type=time]::-webkit-datetime-edit-hour-field,input[type=time]::-webkit-datetime-edit-minute-field,input[type=time]::-webkit-datetime-edit-ampm-field,input[type=date]::-webkit-datetime-edit-text,input[type=time]::-webkit-datetime-edit-text{color:inherit;-webkit-text-fill-color:currentColor;opacity:1;font-weight:inherit}
/* 빈 칸일 때만 옅게 */
input[data-e]::-webkit-datetime-edit,input[data-e]::-webkit-datetime-edit-fields-wrapper,input[data-e]::-webkit-datetime-edit-text,input[data-e]::-webkit-datetime-edit-year-field,input[data-e]::-webkit-datetime-edit-month-field,input[data-e]::-webkit-datetime-edit-day-field,input[data-e]::-webkit-datetime-edit-hour-field,input[data-e]::-webkit-datetime-edit-minute-field,input[data-e]::-webkit-datetime-edit-ampm-field{color:var(--muted,#8a8f98);-webkit-text-fill-color:currentColor;opacity:1}

/* ===== ASSIST 바닥: 위 안전 영역은 화면 맨 위 .top 한 곳에서만 받아요(띠 위 6px, 띠 아래 6px) ===== */
:root{--sat:env(safe-area-inset-top,0px);--sab:env(safe-area-inset-bottom,0px)}
.top{padding-top:calc(var(--sat) + 6px)}
.top .seedbar{margin:0 var(--gutter,16px) 6px}
/* ===== APP CSS ===== */
:root{
  --bg:#f6f4ee;--card:#ffffff;--card2:#ebe8de;--text:#0d0d0d;--muted:#77746a;--line:#d9d6cc;
  --accent:#ff4d00;--on-accent:#ffffff;--danger:#d62d00;--seed-bg:#ffffff;--sheet-bg:#f6f4ee;
  --toast-bg:#0d0d0d;--toast-fg:#f6f4ee;--toast-ac:#ff7a3d;
  --font-head:"Helvetica Neue","Arial Black","Inter","Roboto",system-ui,"Apple SD Gothic Neo","Noto Sans KR",sans-serif;
  --font-mono:"SF Mono","Menlo","Roboto Mono","Courier New",monospace;
  --font-body:system-ui,"Apple SD Gothic Neo","Noto Sans KR",sans-serif;--font-display:var(--font-head);
  --r-card:22px;--gutter:16px;--tab-h:58px;
}
body{word-break:keep-all;overflow-wrap:break-word}
.page.wl{background:#f6f4ee}
.wl .seedbar{border:1.5px solid #0d0d0d;border-radius:8px;color:#0d0d0d;background:#fff}
.wl .seedbar button{color:#d62d00}
.hd{display:flex;align-items:flex-end;justify-content:space-between;margin:12px 18px 0}
.hd .n{display:flex;align-items:flex-end;gap:10px}
.hd .n b{font:900 78px/.82 var(--font-head);letter-spacing:-.04em;font-variant-numeric:tabular-nums}
.hd .n span{font:900 22px/1 var(--font-head);padding-bottom:4px;letter-spacing:-.01em}
.hd .n span small{display:block;font:700 12px/1.3 var(--font-mono);letter-spacing:.14em;color:#77746a;margin-bottom:2px}
.pls{width:56px;height:56px;border-radius:50%;background:#0d0d0d;color:#fff;display:flex;align-items:center;justify-content:center;box-shadow:0 0 0 3px #f6f4ee,0 0 0 5px #ff4d00}
.stk{margin:18px 14px 0}
.cd{position:relative;display:block;width:100%;border-radius:22px;background:var(--cb);color:var(--ci);text-align:start;box-shadow:0 -3px 0 rgba(0,0,0,.08),0 10px 18px -8px rgba(0,0,0,.35)}
.cd.big{padding:16px 16px 16px}
.cd.sm{height:92px;margin-top:-30px;padding:14px 18px 0}
.cd.sm:first-of-type{margin-top:14px}
.cd.big .tp,.cd.sm .tp{display:flex;align-items:center;gap:10px}
.cd .ty{font:700 12px/1 var(--font-mono);letter-spacing:.14em;text-transform:uppercase;padding:5px 8px;border-radius:5px;background:var(--ci);color:var(--cb)}
.cd .nm{flex:1;min-width:0;font:900 22px/1.15 var(--font-head);letter-spacing:-.02em;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}
.cd.big .nm{font-size:30px;white-space:normal;display:-webkit-box;-webkit-line-clamp:2;-webkit-box-orient:vertical}
.cd .ex{flex:none;width:44px;height:44px;border-radius:50%;background:var(--ci);color:var(--cb);display:flex;align-items:center;justify-content:center}
.cd .pn{margin-top:14px;padding:14px 10px 10px;border-radius:12px;background:#fff;color:#0d0d0d;text-align:center;box-shadow:inset 0 0 0 1px rgba(0,0,0,.08)}
.cd .pn svg{display:block;margin:0 auto;max-width:100%;height:auto}
.cd .pn .vl{margin-top:8px;font:700 13px/1.2 var(--font-mono);letter-spacing:.12em;color:#0d0d0d;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}
.cd .hint{margin-top:10px;display:flex;justify-content:space-between;align-items:center;font:700 12px/1 var(--font-mono);letter-spacing:.06em;opacity:.8}
.cd .hint button{height:34px;padding:0 12px;border-radius:17px;box-shadow:inset 0 0 0 1.5px currentColor;font:800 12px/34px var(--font-body);position:relative}
.cd .hint button:before{content:"";position:absolute;left:0;right:0;top:-6px;bottom:-6px}
.cd.pick{cursor:pointer}
.tail{height:30px}
.sec{margin:24px 18px 0;font:800 12px/1 var(--font-mono);letter-spacing:.16em;color:#0d0d0d;text-transform:uppercase}
.big2{margin:14px 18px 0;font:900 38px/1 var(--font-head);letter-spacing:-.03em}
.sub{margin:6px 18px 0;font:600 14px/1.45 var(--font-body);color:#77746a}
.scn{position:relative;margin:18px 18px 0;height:250px;border-radius:22px;background:#0d0d0d;overflow:hidden}
.scn .fr{position:absolute;left:50%;top:42%;width:150px;height:150px;margin:-75px 0 0 -75px}
.scn .fr i{position:absolute;width:34px;height:34px;border:5px solid #fff}
.scn .fr i:nth-child(1){left:0;top:0;border-right:0;border-bottom:0;border-radius:12px 0 0 0}
.scn .fr i:nth-child(2){right:0;top:0;border-left:0;border-bottom:0;border-radius:0 12px 0 0}
.scn .fr i:nth-child(3){left:0;bottom:0;border-right:0;border-top:0;border-radius:0 0 0 12px}
.scn .fr i:nth-child(4){right:0;bottom:0;border-left:0;border-top:0;border-radius:0 0 12px 0}
.scn .ls{position:absolute;left:50%;top:42%;width:190px;height:3px;margin:-1.5px 0 0 -95px;background:#ff4d00;box-shadow:0 0 18px 3px rgba(255,77,0,.8)}
.scn .gb{position:absolute;left:50%;bottom:16px;transform:translateX(-50%);height:50px;padding:0 22px;border-radius:25px;background:#ff4d00;color:#fff;font:900 16px/50px var(--font-head);white-space:nowrap}
.rsl{margin:14px 18px 0;padding:14px 16px;border-radius:14px;background:#fff;box-shadow:inset 0 0 0 1.5px #0d0d0d}
.rsl b{display:block;font:700 15px/1.45 var(--font-mono);word-break:break-all}
.rsl span{display:block;margin-top:6px;font:700 12px/1 var(--font-mono);letter-spacing:.12em;color:#77746a;text-transform:uppercase}
.rsl .bt{display:flex;flex-wrap:wrap;gap:8px;margin-top:12px}.rsl .bt .btn{flex:1 1 40%;min-height:44px;height:auto;border-radius:22px;padding:6px 12px;font:800 14px/1.1 var(--font-body);white-space:normal;text-align:center}
.btn.blk{background:#0d0d0d;color:#fff}.btn.org{background:#ff4d00;color:#fff}.btn.out{background:transparent;box-shadow:inset 0 0 0 1.5px #0d0d0d;color:#0d0d0d}
.alt{margin:12px 18px 0;display:flex;gap:8px}.alt .btn{flex:1;height:48px;border-radius:24px;font:800 14px/1 var(--font-body);white-space:nowrap}
.cf{margin:14px 18px 0}
.cf .pv{margin-top:14px;padding:16px 10px;border-radius:14px;background:#fff;box-shadow:inset 0 0 0 1.5px #0d0d0d;text-align:center;min-height:140px;display:flex;align-items:center;justify-content:center;flex-direction:column;gap:8px}
.cf .pv svg{display:block;max-width:100%;height:auto}
.cf .pv .er{font:700 13px/1.4 var(--font-body);color:#d62d00}
.cf .pv .vl{font:700 12px/1.2 var(--font-mono);letter-spacing:.12em;color:#0d0d0d;max-width:100%;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}
.seg4{display:flex;gap:6px;overflow-x:auto;scrollbar-width:none}.seg4::-webkit-scrollbar{display:none}
.seg4 button{flex:none;min-height:42px;padding:0 14px;border-radius:21px;background:transparent;box-shadow:inset 0 0 0 1.5px #0d0d0d;font:800 14px/42px var(--font-body);white-space:nowrap}
.seg4 button.on{background:#0d0d0d;color:#fff}
.sw{display:inline-block;width:38px;height:38px;border-radius:50%;background:var(--cb);box-shadow:inset 0 0 0 2px rgba(0,0,0,.2);position:relative}
.sws2{display:flex;gap:10px;flex-wrap:wrap}.sws2 button.on{box-shadow:0 0 0 3px #f6f4ee,0 0 0 5px #0d0d0d}
.sws2 button{width:38px;height:38px;border-radius:50%;background:var(--cb);box-shadow:inset 0 0 0 2px rgba(0,0,0,.18);position:relative}
.sws2 button:before{content:"";position:absolute;inset:-4px}
.lb2{display:block;margin:14px 0 6px;font:800 12px/1 var(--font-mono);letter-spacing:.12em;color:#0d0d0d;text-transform:uppercase}
.cf .in{border:1.5px solid #0d0d0d;border-radius:12px;background:#fff}
.nav{display:flex;height:calc(var(--tab-h) + env(safe-area-inset-bottom,0px));padding-bottom:env(safe-area-inset-bottom,0px);background:#0d0d0d;flex:none}
.nv{flex:1;display:flex;flex-direction:column;align-items:center;justify-content:center;gap:3px;color:#8d8a80}
.nv i{font-style:normal;font:800 12px/1 var(--font-head)}
.nv.on{color:#ff6a2a}
.shw{position:fixed;inset:0;z-index:55;background:#fff;color:#0d0d0d;display:flex;flex-direction:column;padding:calc(env(safe-area-inset-top,0px) + 8px) 18px calc(env(safe-area-inset-bottom,0px) + 18px);animation:rin .22s ease-out}
@keyframes rin{from{transform:translateY(20px);opacity:0}to{transform:none;opacity:1}}
.shw .hh{display:flex;align-items:center;gap:10px;min-height:56px}
.shw .hh b{flex:1;font:900 28px/1.1 var(--font-head);letter-spacing:-.02em;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}
.shw .hh button{flex:none;width:48px;height:48px;border-radius:50%;background:#0d0d0d;color:#fff;display:flex;align-items:center;justify-content:center}
.shw .cv{flex:1;min-height:0;display:flex;flex-direction:column;align-items:center;justify-content:center;gap:16px}
.shw .cv svg{display:block;width:100%;max-width:420px;height:auto;max-height:62vh}
.shw .vl{font:700 17px/1.3 var(--font-mono);letter-spacing:.14em;text-align:center;word-break:break-all}
.shw .st{display:flex;align-items:center;gap:8px;font:800 12px/1 var(--font-mono);letter-spacing:.1em;color:#ff4d00;text-transform:uppercase;min-height:16px}
.fld .seg button.on{background:#0d0d0d;color:#fff}
.empty{color:#77746a}.empty b{color:#0d0d0d}
</style>
<style id="byve-ios-date">input[type="date"],input[type="time"],input[type="datetime-local"],input[type="month"],input[type="week"]{display:inline-flex;align-items:center;min-height:2.75em;line-height:normal;-webkit-appearance:none;appearance:none} input[type="date"]::-webkit-date-and-time-value,input[type="time"]::-webkit-date-and-time-value,input[type="datetime-local"]::-webkit-date-and-time-value,input[type="month"]::-webkit-date-and-time-value,input[type="week"]::-webkit-date-and-time-value{text-align:start;margin:0;min-height:1.2em} input[type="date"]::-webkit-datetime-edit,input[type="time"]::-webkit-datetime-edit,input[type="datetime-local"]::-webkit-datetime-edit,input[type="month"]::-webkit-datetime-edit,input[type="week"]::-webkit-datetime-edit{padding:0;line-height:normal}</style><style id="byve-seed-look">:root{--card2:#ebdfde;--accent:#ff006d;--danger:#d6006f;--toast-ac:#ff3d8e}:where([class*="day"],[class*="cell"],[class*="slot"])>:where(span,small,b,em,i){min-width:0;max-width:100%;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}</style><style data-byve-server-text-safety>input:not([type=number]):not([inputmode=decimal]):not([inputmode=numeric]),textarea,select,[contenteditable]{unicode-bidi:plaintext}</style><style data-byve-server-transient-overlay>:where([class*="toast" i],[class*="snackbar" i],[id*="toast" i],[id*="snackbar" i]){pointer-events:none!important}:where([class*="toast" i],[class*="snackbar" i],[id*="toast" i],[id*="snackbar" i]) :where(button,a,input,select,textarea,[role="button"],[data-action]){pointer-events:auto!important}</style><script data-byve-polish>(function(){var s=document,u=innerHeight,c,E=0,x,M={},$=0,N=0;if(window.__byvePolish)return;window.__byvePolish=1;var F="data-bp",m="data-bb",R="data-be",A="data-bk",C="input:not([type]),[type=text],[type=search],[type=email],[type=tel],[type=number]",w="[type=date],[type=time],[type=datetime-local],[type=month],[type=week]",G="form,dialog,[role=dialog],[class*=modal],[class*=sheet]";function b(t){return getComputedStyle(t)}function l(t){return parseFloat(t)||0}function p(t){return t.getBoundingClientRect()}function S(t){var e=p(t),i;return e.width<24||e.height<8?0:(i=b(t),i.visibility!="hidden"&&i.opacity>.1)}function J(t){return!t||/, 0\)$/.test(t)}function q(t){var e=b(t);return{h:p(t).height,bw:e.borderTopWidth,bc:e.borderTopColor,br:e.borderTopLeftRadius,bg:e.backgroundColor,fs:e.fontSize,fw:e.fontWeight,ff:e.fontFamily,c:e.color,pl:e.paddingLeft,pr:e.paddingRight,ap:e.webkitAppearance,d:e.display}}function T(t,e){for(var i=t.querySelectorAll(e),r=0;r<i.length;r++)if(S(i[r]))return q(i[r])}function Q(t){var e=t.closest(G)||s.body,i=T(e,C)||T(s.body,C)||T(s.body,"textarea");return i&&t.tagName!="SELECT"&&i.h>60&&(i.h=0),i}function V(t){var e=t.parentElement;return t.closest("form,label")||t.labels&&t.labels.length||e&&e.querySelector(C+",textarea")}function X(t,e,i){return t.tagName=="SELECT"&&e.ap!="none"||e.h<43?1:i&&(i.h&&i.h<61&&Math.abs(e.h-i.h)>2||e.bw!=i.bw||Math.abs(l(e.br)-l(i.br))>1||e.bg!=i.bg||Math.abs(l(e.fs)-l(i.fs))>.5)}function j(t,e){var i=b(t.parentElement||s.body).color,r=i.match(/[\d.]+/g)||[0,0,0];return e.h=48,e.bw="1px",e.bc="rgba("+r.slice(0,3)+",.28)",e.br=l(e.br)?e.br:"10px",e.fs=Math.max(16,l(e.fs))+"px",e.c=i,e.pl=e.pr="14px",e}function tt(t,e){var i=e>0?e:Math.max(44,Math.round(t.h&&t.h<61?t.h:48)),r=Math.max(l(t.pr),12),a=[e=="k"?"k":i,t.bw,t.bc,t.br,t.bg,t.fs,t.fw,t.ff,t.c,t.pl,t.pr].join("|"),n,o;return M[a]?M[a]:(n=M[a]=++$,o='[data-bp="'+n+'"][data-bp][data-bp]',e=="k"?(c.textContent+=o+"{"+("border-width:"+t.bw+";border-style:solid;border-radius:"+t.br+";background-color:"+t.bg+";color:"+t.c+";").replace(/;/g,"!important;")+"}"+o+":not(:focus){border-color:"+t.bc+"!important}",n):(c.textContent+=o+"{"+("box-sizing:border-box;-webkit-appearance:none;height:"+i+"px;min-height:"+i+"px;border-width:"+t.bw+";border-style:solid;border-radius:"+t.br+";background-color:"+t.bg+";font-size:"+t.fs+";font-weight:"+t.fw+";font-family:"+t.ff+";color:"+t.c+";padding:0 "+t.pr+" 0 "+t.pl+";line-height:normal;").replace(/;/g,"!important;")+"}"+o+":not(:focus){border-color:"+t.bc+"!important}select"+o+"{padding-right:"+(r+22)+"px!important;background:"+t.bg+" no-repeat right "+r+`px center/12px 8px url("data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 12 8'><path d='M1 1.5l5 5 5-5' fill='none' stroke='`+t.c+`' stroke-width='1.8'/></svg>")!important;text-overflow:ellipsis}`,n))}function et(t,e,i){var r=p(t).width,a=t.tagName=="SELECT",n=a?Math.max(l(i.pr),12)+22:l(i.pr),o=t.parentElement,d=o&&b(o),g;return r-l(i.pl)-n-2*l(i.bw)<48?"k":(g=o&&[].some.call(o.children,function(f){return f!=t&&f.matches("input,select,textarea,button")&&S(f)}),g&&/flex/.test(d.display)&&!/column/.test(d.flexDirection)&&e.h<43?Math.max(24,Math.round(e.h)):0)}function it(t){var e=b(t),i=t.options&&t.options[t.selectedIndex],r=s.createElement("canvas").getContext("2d"),a,n=t.parentElement;!i||!r||(r.font=e.fontWeight+" "+e.fontSize+" "+e.fontFamily,a=Math.ceil(r.measureText(i.text).width+l(e.paddingLeft)+l(e.paddingRight)+2*l(e.borderLeftWidth)+36),!(p(t).width+1>=a)&&(t.style.setProperty("min-width",Math.min(a,innerWidth-32)+"px"),t.style.setProperty("flex-shrink","0"),n&&/flex/.test(b(n).display)&&n.scrollWidth>n.clientWidth+1&&n.style.setProperty("flex-wrap","wrap")))}function nt(){var t=s.body.querySelectorAll("select:not([multiple]),"+w),e,i,r,a,n,o;for(e=0;e<t.length&&e<400;e++)i=t[e],n=i.tagName=="INPUT",o=i.hasAttribute(F),n&&i.toggleAttribute(R,!i.value),S(i)&&(r=q(i),n&&!i.hasAttribute("data-bd")&&i.setAttribute("data-bd",/inline/.test(r.d)?"i":"b"),!(!o&&!V(i))&&(a=Q(i),(o?a:X(i,r,a))&&(a=a||j(i,r),o||(i.setAttribute(A,et(i,r,a)),i.getAttribute(A)=="k"&&it(i)),i.setAttribute(F,tt(a,i.getAttribute(A))))))}function ot(){var t=s.body.querySelectorAll("*"),e=innerWidth,i=[],r=[],a,n,o,d,g;for(u=innerHeight,a=0;a<t.length&&a<3e3;a++)n=t[a],o=b(n),!(o.position!="fixed"&&!(o.position=="absolute"&&o.bottom!="auto"&&l(o.bottom)<4))&&(d=p(n),!(d.height<24||d.height>u*.35||d.width<e*.5||d.top<u*.45||o.position=="fixed"&&d.bottom<u-2)&&(g=s.elementFromPoint(d.left+d.width/2,Math.min(u-2,d.top+6)),g&&n.contains(g)&&!i.some(function(f){return f.contains(n)})&&i.push(n)));i.forEach(function(f){var y=p(f),B=[],Y=s.scrollingElement;for(b(f).position=="fixed"&&Y.scrollHeight>u+2&&B.push(s.body),a=0;a<t.length&&a<3e3;a++)n=t[a],n.scrollHeight>n.clientHeight+4&&!n.contains(f)&&/auto|scroll/.test(b(n).overflowY)&&(d=p(n),d.bottom>y.top+2&&d.right>y.left&&d.left<y.right&&B.push(n));B.forEach(function(h){if(!(r.indexOf(h)>=0)){r.push(h);for(var v=h==s.body,I=v?{top:-scrollY,bottom:u}:p(h),rt=v?0:h.scrollTop,K=l(h.getAttribute(m)),U=h.hasAttribute(m)?l(h.getAttribute("data-bb0")):l(b(h).paddingBottom),Z=(v?Y.scrollHeight:h.scrollHeight)-K,L=0,H=s.createTreeWalker(h,1),at,P,k,W;n=H.nextNode();)if(!f.contains(n)){if(o=b(n),o.position=="fixed"||o.display=="none"||o.visibility=="hidden"){z(H,n);continue}d=p(n),!(d.width<2||d.height<2||d.height>Z*.9&&n.children.length)&&(P=!n.children.length||n.matches("input,textarea,select,button,img")||(!J(o.backgroundColor)||l(o.borderBottomWidth))&&l(o.paddingBottom)<48,/auto|scroll/.test(o.overflowY)&&n.scrollHeight>n.clientHeight+4&&(P=1,z(H,n)),P&&(L=Math.max(L,d.bottom-I.top+rt)))}W=L+Math.min(I.bottom,u)-y.top+16+(y.bottom>=u-2?N:0),k=W>(v?u:h.clientHeight)?Math.max(0,Math.ceil(W-Z)):0,!(Math.abs(k-K)<2)&&(h.hasAttribute(m)||h.setAttribute("data-bb0",U),h.setAttribute(m,k),h.style.setProperty("padding-bottom",U+k+"px","important"))}})})}function z(t,e){for(t.currentNode=e;t.lastChild(););}function D(){E=0;try{nt()}catch(t){}try{ot()}catch(t){}x&&x.takeRecords()}function O(){E=E||setTimeout(D,120)}function _(){var t=s.createElement("i");c=s.createElement("style"),s.head.appendChild(c),c.textContent="input[data-bd][data-bd]:not([hidden]){display:inline-flex;align-items:center;line-height:normal}input[data-bd=b][data-bd]:not([hidden]){display:flex}[data-bp][data-be]::-webkit-datetime-edit{opacity:.55}:where("+w+")::-webkit-date-and-time-value{text-align:start;margin:0;min-height:1.2em}:where("+w+")::-webkit-datetime-edit{padding:0;line-height:normal}",t.style.cssText="position:fixed;padding-bottom:env(safe-area-inset-bottom)",s.body.appendChild(t),N=l(b(t).paddingBottom),t.remove(),D(),x=new MutationObserver(function(e){for(var i=0,r;r=e[i];i++)if(r.target!=c&&!(r.attributeName=="style"&&r.target.hasAttribute(m)))return O()}),x.observe(s.documentElement,{subtree:!0,childList:!0,attributes:!0,attributeFilter:["class","style","hidden","data-byve-theme"]}),["resize","load","transitionend","change"].forEach(function(e){addEventListener(e,O,!0)}),s.addEventListener("input",function(e){e=e.target,e.matches&&e.matches(w)&&e.toggleAttribute(R,!e.value)},!0)}s.readyState=="loading"?s.addEventListener("DOMContentLoaded",_):_()})();</script></head>
<body>
<div id="app"><div class="page wl" id="page"></div><nav class="nav" id="nav"></nav></div>
<script>
/* ===== ICONS(쓰는 것만) ===== */
const ICONS={
'arrow-r':'<path d="M5 12h14M13 6l6 6-6 6"/>',
'camera':'<path d="M4 8.500A2.500 2.500 0 0 1 6.500 6H8l1.500-2h5L16 6h1.500A2.500 2.500 0 0 1 20 8.500v8a2.500 2.500 0 0 1-2.500 2.500h-11A2.500 2.500 0 0 1 4 16.500z"/><circle cx="12" cy="12.500" r="3.500"/>',
'check':'<path d="m5 12.5 4.6 4.6L19 7.6"/>',
'copy':'<rect x="8.500" y="8.500" width="11" height="11" rx="2.500"/><path d="M15.500 8.500V6.500A2.500 2.500 0 0 0 13 4H6.500A2.500 2.500 0 0 0 4 6.500V13a2.500 2.500 0 0 0 2.500 2.500h2"/>',
'edit':'<path d="M4.500 19.500l1-4.200L16.300 4.500a2 2 0 0 1 2.800 0l.4.400a2 2 0 0 1 0 2.800L8.700 18.500z"/><path d="m14.500 6.300 3.200 3.200"/>',
'grid':'<rect x="4" y="4" width="7" height="7" rx="2"/><rect x="13" y="4" width="7" height="7" rx="2"/><rect x="4" y="13" width="7" height="7" rx="2"/><rect x="13" y="13" width="7" height="7" rx="2"/>',
'layers':'<path d="m12 4 8.500 4.500L12 13 3.500 8.500z"/><path d="m3.500 12.500 8.500 4.500 8.500-4.500"/>',
'pen':'<path d="m4.500 19.500.8-4L16.500 4.300a1.800 1.800 0 0 1 2.500 0l.7.7a1.800 1.800 0 0 1 0 2.500L8.500 18.700z"/><path d="m14.500 6.300 3.200 3.200"/>',
'plus':'<path d="M12 5v14M5 12h14"/>',
'trash':'<path d="M5 7h14M10 7V4.500h4V7M6.500 7l.8 12.500h9.400L17.500 7M10 11v5M14 11v5"/>',
'x':'<path d="M6.5 6.5l11 11M17.5 6.5l-11 11"/>'
};
/*ICONS: plus x check trash copy edit camera pen grid layers arrow-r*/
/* ===== LIB qr ===== */
  var QR = (function () {
    var ECW = [
      [7, 10, 15, 20, 26, 18, 20, 24, 30, 18, 20, 24, 26, 30, 22, 24, 28, 30, 28, 28, 28, 28, 30, 30, 26, 28, 30, 30, 30, 30, 30, 30, 30, 30, 30, 30, 30, 30, 30, 30],
      [10, 16, 26, 18, 24, 16, 18, 22, 22, 26, 30, 22, 22, 24, 24, 28, 28, 26, 26, 26, 26, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28],
      [13, 22, 18, 26, 18, 24, 18, 22, 20, 24, 28, 26, 24, 20, 30, 24, 28, 28, 26, 30, 28, 30, 30, 30, 30, 28, 30, 30, 30, 30, 30, 30, 30, 30, 30, 30, 30, 30, 30, 30],
      [17, 28, 22, 16, 22, 28, 26, 26, 24, 28, 24, 28, 22, 24, 24, 30, 28, 28, 26, 28, 30, 24, 30, 30, 30, 30, 30, 30, 30, 30, 30, 30, 30, 30, 30, 30, 30, 30, 30, 30]];
    var NBL = [
      [1, 1, 1, 1, 1, 2, 2, 2, 2, 4, 4, 4, 4, 4, 6, 6, 6, 6, 7, 8, 8, 9, 9, 10, 12, 12, 12, 13, 14, 15, 16, 17, 18, 19, 19, 20, 21, 22, 24, 25],
      [1, 1, 1, 2, 2, 4, 4, 4, 5, 5, 5, 8, 9, 9, 10, 10, 11, 13, 14, 16, 17, 17, 18, 20, 21, 23, 25, 26, 28, 29, 31, 33, 35, 37, 38, 40, 43, 45, 47, 49],
      [1, 1, 2, 2, 4, 4, 6, 6, 8, 8, 8, 10, 12, 16, 12, 17, 16, 18, 21, 20, 23, 23, 25, 27, 29, 34, 34, 35, 38, 40, 43, 45, 48, 51, 53, 56, 59, 62, 65, 68],
      [1, 1, 2, 4, 4, 4, 5, 6, 8, 8, 11, 11, 16, 16, 18, 16, 19, 21, 25, 25, 25, 34, 30, 32, 35, 37, 40, 42, 45, 48, 51, 54, 57, 60, 63, 66, 70, 74, 77, 81]];
    var LV = { L: 0, M: 1, Q: 2, H: 3 }, LVN = ['L', 'M', 'Q', 'H'], FMT = [1, 0, 3, 2];
    var ALNUM = '0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ $%*+-./:';
    var EXP = [], LOG = [], i, x = 1;
    for (i = 0; i < 255; i++) { EXP[i] = x; LOG[x] = i; x <<= 1; if (x & 256) x ^= 0x11D; }
    for (i = 255; i < 512; i++) EXP[i] = EXP[i - 255];
    function gmul(a, b) { return a && b ? EXP[LOG[a] + LOG[b]] : 0; }
    function ginv(a) { return EXP[255 - LOG[a]]; }
    function rawModules(v) { var r = (16 * v + 128) * v + 64, n; if (v >= 2) { n = Math.floor(v / 7) + 2; r -= (25 * n - 10) * n - 55; if (v >= 7) r -= 36; } return r; }
    function dataCodewords(v, l) { return Math.floor(rawModules(v) / 8) - ECW[l][v - 1] * NBL[l][v - 1]; }
    function utf8(s) { var o = [], c, n; s = String(s); for (n = 0; n < s.length; n++) { c = s.codePointAt(n); if (c > 0xFFFF) n++; if (c < 0x80) o.push(c); else if (c < 0x800) o.push(0xC0 | c >> 6, 0x80 | c & 63); else if (c < 0x10000) o.push(0xE0 | c >> 12, 0x80 | c >> 6 & 63, 0x80 | c & 63); else o.push(0xF0 | c >> 18, 0x80 | c >> 12 & 63, 0x80 | c >> 6 & 63, 0x80 | c & 63); } return o; }
    function unutf8(b) {
      var s = '', n = 0, c, k, need;
      while (n < b.length) {
        c = b[n++];
        if (c < 0x80) need = 0; else if (c >= 0xC2 && c < 0xE0) { need = 1; c &= 31; } else if (c >= 0xE0 && c < 0xF0) { need = 2; c &= 15; } else if (c >= 0xF0 && c < 0xF5) { need = 3; c &= 7; } else return null;
        for (k = 0; k < need; k++) { if (n >= b.length || (b[n] & 0xC0) !== 0x80) return null; c = c << 6 | b[n++] & 63; }
        s += String.fromCodePoint(c);
      }
      return s;
    }
    function latin1(b) { var s = '', n; for (n = 0; n < b.length; n++) s += String.fromCharCode(b[n]); return s; }
    function rsDiv(deg) { var r = [], n, j, root = 1; for (n = 0; n < deg - 1; n++) r.push(0); r.push(1); for (n = 0; n < deg; n++) { for (j = 0; j < deg; j++) { r[j] = gmul(r[j], root); if (j + 1 < deg) r[j] ^= r[j + 1]; } root = gmul(root, 2); } return r; }
    function rsRem(data, div) { var r = div.map(function () { return 0; }), n, j, f; for (n = 0; n < data.length; n++) { f = data[n] ^ r.shift(); r.push(0); for (j = 0; j < div.length; j++) r[j] ^= gmul(div[j], f); } return r; }
    /* error correction of one block (data+ecc, in place). returns fixed count or -1 */
    function rsFix(msg, nec) {
      var n = msg.length, syn = [], a, j, any = 0, s, p;
      function synd() { any = 0; syn = []; for (a = 0; a < nec; a++) { s = 0; for (j = 0; j < n; j++) s = gmul(s, EXP[a]) ^ msg[j]; syn.push(s); if (s) any = 1; } }
      synd();
      if (!any) return 0;
      var C = [1], B = [1], L = 0, m = 1, b = 1, d, T, cf;
      for (a = 0; a < nec; a++) {
        d = syn[a];
        for (j = 1; j <= L; j++) d ^= gmul(C[j] || 0, syn[a - j]);
        if (!d) { m++; continue; }
        T = C.slice(); cf = gmul(d, ginv(b));
        for (j = 0; j < B.length; j++) C[j + m] = (C[j + m] || 0) ^ gmul(cf, B[j]);
        for (j = 0; j < C.length; j++) C[j] = C[j] || 0;
        if (2 * L <= a) { L = a + 1 - L; B = T; b = d; m = 1; } else m++;
      }
      if (L * 2 > nec) return -1;
      var pos = [], xi, v;
      for (p = 0; p < n; p++) { xi = EXP[(255 - p) % 255]; v = 0; for (j = L; j >= 0; j--) v = gmul(v, xi) ^ (C[j] || 0); if (!v) pos.push(p); }
      if (pos.length !== L) return -1;
      var om = [], o;
      for (a = 0; a < nec; a++) { o = 0; for (j = 0; j <= a && j <= L; j++) o ^= gmul(C[j] || 0, syn[a - j]); om.push(o); }
      pos.forEach(function (pp) {
        var X = EXP[pp % 255], Xi = EXP[(255 - pp) % 255], nu = 0, de = 0, k, pw = 1;
        for (k = om.length - 1; k >= 0; k--) nu = gmul(nu, Xi) ^ om[k];
        for (k = 1; k <= L; k += 2) { de ^= gmul(C[k] || 0, pw); pw = gmul(pw, gmul(Xi, Xi)); }
        if (de) msg[n - 1 - pp] ^= gmul(X, gmul(nu, ginv(de)));
      });
      synd();
      return any ? -1 : L;
    }
    function alignPos(v) { if (v === 1) return []; var n = Math.floor(v / 7) + 2, size = v * 4 + 17, step = v === 32 ? 26 : Math.ceil((v * 4 + 4) / (n * 2 - 2)) * 2, r = [6], p; for (p = size - 7; r.length < n; p -= step) r.splice(1, 0, p); return r; }
    function fmtBits(l, mask) { var d = FMT[l] << 3 | mask, r = d, n; for (n = 0; n < 10; n++) r = r << 1 ^ (r >>> 9) * 0x537; return (d << 10 | r) ^ 0x5412; }
    function verBits(v) { var r = v, n; for (n = 0; n < 12; n++) r = r << 1 ^ (r >>> 11) * 0x1F25; return v << 12 | r; }
    function maskAt(k, x, y) {
      switch (k) {
        case 0: return (x + y) % 2 === 0; case 1: return y % 2 === 0; case 2: return x % 3 === 0; case 3: return (x + y) % 3 === 0;
        case 4: return (Math.floor(x / 3) + Math.floor(y / 2)) % 2 === 0; case 5: return x * y % 2 + x * y % 3 === 0;
        case 6: return (x * y % 2 + x * y % 3) % 2 === 0; default: return ((x + y) % 2 + x * y % 3) % 2 === 0;
      }
    }
    /* empty matrix with function patterns; fn[y][x]=1 where data may not go */
    function frame(v) {
      var size = v * 4 + 17, m = [], fn = [], y, x2, a, b, al = alignPos(v), dx, dy, d;
      for (y = 0; y < size; y++) { m.push(new Uint8Array(size)); fn.push(new Uint8Array(size)); }
      function set(xx, yy, dark) { if (xx < 0 || yy < 0 || xx >= size || yy >= size) return; m[yy][xx] = dark ? 1 : 0; fn[yy][xx] = 1; }
      for (a = 0; a < size; a++) { set(6, a, a % 2 === 0); set(a, 6, a % 2 === 0); }
      [[3, 3], [size - 4, 3], [3, size - 4]].forEach(function (c) { for (dy = -4; dy <= 4; dy++) for (dx = -4; dx <= 4; dx++) { d = Math.max(Math.abs(dx), Math.abs(dy)); set(c[0] + dx, c[1] + dy, d !== 2 && d !== 4); } });
      for (a = 0; a < al.length; a++) for (b = 0; b < al.length; b++) {
        if ((a === 0 && b === 0) || (a === 0 && b === al.length - 1) || (a === al.length - 1 && b === 0)) continue;
        for (dy = -2; dy <= 2; dy++) for (dx = -2; dx <= 2; dx++) set(al[a] + dx, al[b] + dy, Math.max(Math.abs(dx), Math.abs(dy)) !== 1);
      }
      for (a = 0; a < 9; a++) { if (!fn[8][a]) set(a, 8, 0); if (!fn[a][8]) set(8, a, 0); }
      for (a = 0; a < 8; a++) { set(size - 1 - a, 8, 0); set(8, size - 1 - a, 0); }
      set(8, size - 8, 1);
      if (v >= 7) for (a = 0; a < 18; a++) { x2 = size - 11 + a % 3; b = Math.floor(a / 3); set(x2, b, 0); set(b, x2, 0); }
      return { m: m, fn: fn, size: size, set: set };
    }
    function putFormat(f, l, mask) {
      var bits = fmtBits(l, mask), size = f.size, a, bit = function (k) { return bits >>> k & 1; };
      for (a = 0; a <= 5; a++) f.set(8, a, bit(a));
      f.set(8, 7, bit(6)); f.set(8, 8, bit(7)); f.set(7, 8, bit(8));
      for (a = 9; a < 15; a++) f.set(14 - a, 8, bit(a));
      for (a = 0; a < 8; a++) f.set(size - 1 - a, 8, bit(a));
      for (a = 8; a < 15; a++) f.set(8, size - 15 + a, bit(a));
      f.set(8, size - 8, 1);
    }
    function zig(f, cb) {
      var size = f.size, right, vert, j, xx, yy, up, k = 0;
      for (right = size - 1; right >= 1; right -= 2) {
        if (right === 6) right = 5;
        for (vert = 0; vert < size; vert++) for (j = 0; j < 2; j++) {
          xx = right - j; up = (right + 1 & 2) === 0; yy = up ? size - 1 - vert : vert;
          if (!f.fn[yy][xx]) cb(xx, yy, k++);
        }
      }
      return k;
    }
    function penalty(m, size) {
      var p = 0, y, x2, run, col, dark = 0, a, k, hist;
      function fin(h) { var n = h[1], core = n > 0 && h[2] === n && h[3] === n * 3 && h[4] === n && h[5] === n; return (core && h[0] >= n * 4 && h[6] >= n ? 1 : 0) + (core && h[6] >= n * 4 && h[0] >= n ? 1 : 0); }
      function line(get) {
        col = 0; run = 0; hist = [0, 0, 0, 0, 0, 0, 0];
        function add(r) { if (hist[0] === 0) r += size; hist.pop(); hist.unshift(r); }
        for (a = 0; a < size; a++) {
          if (get(a) === col) { run++; if (run === 5) p += 3; else if (run > 5) p++; }
          else { add(run); if (!col) p += fin(hist) * 40; col = get(a); run = 1; }
        }
        if (col) { add(run); run = 0; } run += size; add(run); p += fin(hist) * 40;
      }
      for (y = 0; y < size; y++) line(function (k2) { return m[y][k2]; });
      for (x2 = 0; x2 < size; x2++) line(function (k2) { return m[k2][x2]; });
      for (y = 0; y < size - 1; y++) for (x2 = 0; x2 < size - 1; x2++) { k = m[y][x2]; if (k === m[y][x2 + 1] && k === m[y + 1][x2] && k === m[y + 1][x2 + 1]) p += 3; }
      for (y = 0; y < size; y++) for (x2 = 0; x2 < size; x2++) dark += m[y][x2];
      k = Math.ceil(Math.abs(dark * 20 - size * size * 10) / (size * size)) - 1;
      return p + k * 10;
    }
    function modeOf(s) { if (/^[0-9]+$/.test(s)) return 1; var n; for (n = 0; n < s.length; n++) if (ALNUM.indexOf(s.charAt(n)) < 0) return 4; return s.length ? 2 : 4; }
    function ccBits(mode, v) { var g = v < 10 ? 0 : v < 27 ? 1 : 2; return mode === 1 ? [10, 12, 14][g] : mode === 2 ? [9, 11, 13][g] : [8, 16, 16][g]; }
    function encode(text, o) {
      o = o || {}; text = String(text == null ? '' : text);
      var l = LV[String(o.ecc || 'M').toUpperCase()]; if (l == null) l = 1;
      var mode = modeOf(text), bytes = mode === 4 ? utf8(text) : null, count = mode === 4 ? bytes.length : text.length, bits = [], v, n, need;
      function push(val, len) { for (var k = len - 1; k >= 0; k--) bits.push(val >>> k & 1); }
      function payload() { return mode === 1 ? Math.floor(count / 3) * 10 + [0, 4, 7][count % 3] : mode === 2 ? Math.floor(count / 2) * 11 + count % 2 * 6 : count * 8; }
      for (v = Math.max(1, Math.min(40, Math.round(o.minVersion || 1))); v <= 40; v++) { need = 4 + ccBits(mode, v) + payload(); if (need <= dataCodewords(v, l) * 8) break; }
      if (v > 40) return null;
      push(mode, 4); push(count, ccBits(mode, v));
      if (mode === 1) for (n = 0; n < count; n += 3) { var part = text.substr(n, 3); push(parseInt(part, 10), part.length * 3 + 1); }
      else if (mode === 2) for (n = 0; n < count; n += 2) { if (n + 1 < count) push(ALNUM.indexOf(text.charAt(n)) * 45 + ALNUM.indexOf(text.charAt(n + 1)), 11); else push(ALNUM.indexOf(text.charAt(n)), 6); }
      else for (n = 0; n < count; n++) push(bytes[n], 8);
      var cap = dataCodewords(v, l) * 8, data = [], pad = 0xEC;
      push(0, Math.min(4, cap - bits.length)); push(0, (8 - bits.length % 8) % 8);
      for (n = 0; n < bits.length; n += 8) data.push(bits[n] << 7 | bits[n + 1] << 6 | bits[n + 2] << 5 | bits[n + 3] << 4 | bits[n + 4] << 3 | bits[n + 5] << 2 | bits[n + 6] << 1 | bits[n + 7]);
      while (data.length < cap / 8) { data.push(pad); pad ^= 0xEC ^ 0x11; }
      /* blocks */
      var nb = NBL[l][v - 1], ecl = ECW[l][v - 1], rawCw = Math.floor(rawModules(v) / 8), nShort = nb - rawCw % nb, shortLen = Math.floor(rawCw / nb), blocks = [], div = rsDiv(ecl), k = 0, dat, all = [], j;
      for (n = 0; n < nb; n++) { dat = data.slice(k, k + shortLen - ecl + (n < nShort ? 0 : 1)); k += dat.length; var ec = rsRem(dat, div); if (n < nShort) dat.push(0); blocks.push(dat.concat(ec)); }
      for (n = 0; n < blocks[0].length; n++) for (j = 0; j < nb; j++) if (n !== shortLen - ecl || j >= nShort) all.push(blocks[j][n]);
      var f = frame(v), size = f.size, best = -1, bestP = Infinity, mk, yy, xx, pz;
      zig(f, function (x3, y3, idx) { f.m[y3][x3] = idx < all.length * 8 ? all[idx >>> 3] >>> (7 - (idx & 7)) & 1 : 0; });
      if (v >= 7) { var vb = verBits(v); for (n = 0; n < 18; n++) { var bt = vb >>> n & 1, ax = size - 11 + n % 3, bx = Math.floor(n / 3); f.set(ax, bx, bt); f.set(bx, ax, bt); } }
      function apply(mm) { for (yy = 0; yy < size; yy++) for (xx = 0; xx < size; xx++) if (!f.fn[yy][xx] && maskAt(mm, xx, yy)) f.m[yy][xx] ^= 1; }
      var fixed = o.mask != null && o.mask >= 0 && o.mask < 8 ? Math.floor(o.mask) : -1;
      if (fixed >= 0) best = fixed;
      else for (mk = 0; mk < 8; mk++) { apply(mk); putFormat(f, l, mk); pz = penalty(f.m, size); if (pz < bestP) { bestP = pz; best = mk; } apply(mk); }
      apply(best); putFormat(f, l, best);
      return { version: v, size: size, ecc: LVN[l], mask: best, mode: mode === 1 ? 'numeric' : mode === 2 ? 'alphanumeric' : 'byte', modules: f.m, dataCodewords: cap / 8, usedBits: 4 + ccBits(mode, v) + payload() };
    }
    /* module matrix (array of rows, truthy = dark) -> {text, version, ecc, mask, fixed} or null */
    function decode(mod) {
      var size = mod.length, v = (size - 17) / 4, n, j, k;
      if (v !== Math.floor(v) || v < 1 || v > 40) return null;
      function g(x2, y2) { return mod[y2][x2] ? 1 : 0; }
      var raw = 0, raw2 = 0;
      for (n = 0; n <= 5; n++) raw |= g(8, n) << n;
      raw |= g(8, 7) << 6 | g(8, 8) << 7 | g(7, 8) << 8;
      for (n = 9; n < 15; n++) raw |= g(14 - n, 8) << n;
      for (n = 0; n < 8; n++) raw2 |= g(size - 1 - n, 8) << n;
      for (n = 8; n < 15; n++) raw2 |= g(8, size - 15 + n) << n;
      var bestD = 99, bl = 0, bm = 0, cand, dist, l, mk;
      for (l = 0; l < 4; l++) for (mk = 0; mk < 8; mk++) {
        cand = fmtBits(l, mk);
        [raw, raw2].forEach(function (rw) { dist = 0; var xr = cand ^ rw; while (xr) { dist += xr & 1; xr >>>= 1; } if (dist < bestD) { bestD = dist; bl = l; bm = mk; } });
      }
      if (bestD > 3) return null;
      var f = frame(v), bitsArr = [], total = Math.floor(rawModules(v) / 8);
      zig(f, function (x3, y3) { bitsArr.push(g(x3, y3) ^ (maskAt(bm, x3, y3) ? 1 : 0)); });
      var cw = [];
      for (n = 0; n < total; n++) { k = 0; for (j = 0; j < 8; j++) k = k << 1 | bitsArr[n * 8 + j]; cw.push(k); }
      var nb = NBL[bl][v - 1], ecl = ECW[bl][v - 1], nShort = nb - total % nb, shortLen = Math.floor(total / nb), blocks = [], idx = 0, fixed = 0, r;
      for (n = 0; n < nb; n++) blocks.push([]);
      for (n = 0; n < shortLen + 1; n++) for (j = 0; j < nb; j++) { if (n === shortLen - ecl && j < nShort) continue; blocks[j].push(cw[idx++]); }
      var data = [];
      for (n = 0; n < nb; n++) { r = rsFix(blocks[n], ecl); if (r < 0) return null; fixed += r; data = data.concat(blocks[n].slice(0, blocks[n].length - ecl)); }
      var bp = 0, out = '', bytes = [], mode, cnt;
      function take(len) { var val = 0, q; for (q = 0; q < len; q++) { val = val << 1 | (bp < data.length * 8 ? data[bp >>> 3] >>> (7 - (bp & 7)) & 1 : 0); bp++; } return val; }
      function flush() { if (bytes.length) { var s = unutf8(bytes); out += s == null ? latin1(bytes) : s; bytes = []; } }
      while (bp + 4 <= data.length * 8) {
        mode = take(4);
        if (mode === 0) break;
        if (mode === 7) { var e1 = take(8); if (e1 & 0x80) { take(8); if (e1 & 0x40) take(8); } continue; }
        if (mode !== 1 && mode !== 2 && mode !== 4) return null;
        cnt = take(ccBits(mode, v));
        if (mode === 4) { for (n = 0; n < cnt; n++) bytes.push(take(8)); continue; }
        flush();
        if (mode === 1) { for (n = 0; n + 3 <= cnt; n += 3) { k = String(take(10)); out += '000'.slice(k.length) + k; } if (cnt - n === 2) { k = String(take(7)); out += '00'.slice(k.length) + k; } else if (cnt - n === 1) out += String(take(4)); }
        else { for (n = 0; n + 2 <= cnt; n += 2) { k = take(11); out += ALNUM.charAt(Math.floor(k / 45)) + ALNUM.charAt(k % 45); } if (n < cnt) out += ALNUM.charAt(take(6)); }
      }
      flush();
      return { text: out, version: v, ecc: LVN[bl], mask: bm, fixed: fixed, size: size };
    }
    /* ----- photo reader: finder patterns -> perspective grid -> decode. Flat, sharp pictures; QR only. ----- */
    function homography(src, dst) {
      var A = [], n, r, c, k, piv, t;
      for (n = 0; n < 4; n++) {
        var sx = src[n][0], sy = src[n][1], dx = dst[n][0], dy = dst[n][1];
        A.push([sx, sy, 1, 0, 0, 0, -sx * dx, -sy * dx, dx]); A.push([0, 0, 0, sx, sy, 1, -sx * dy, -sy * dy, dy]);
      }
      for (c = 0; c < 8; c++) {
        piv = c; for (r = c + 1; r < 8; r++) if (Math.abs(A[r][c]) > Math.abs(A[piv][c])) piv = r;
        if (Math.abs(A[piv][c]) < 1e-12) return null;
        t = A[c]; A[c] = A[piv]; A[piv] = t;
        for (r = 0; r < 8; r++) if (r !== c) { k = A[r][c] / A[c][c]; if (k) for (n = c; n < 9; n++) A[r][n] -= k * A[c][n]; }
      }
      var hh = []; for (n = 0; n < 8; n++) hh.push(A[n][8] / A[n][n]);
      return function (px, py) { var w = hh[6] * px + hh[7] * py + 1; return [(hh[0] * px + hh[1] * py + hh[2]) / w, (hh[3] * px + hh[4] * py + hh[5]) / w]; };
    }
    function read(img) {
      if (!img || !img.data || !img.width) return null;
      var w = img.width, h = img.height, d = img.data, gray = new Uint8Array(w * h), n, p, x2, y2;
      for (n = 0, p = 0; n < w * h; n++, p += 4) gray[n] = d[p + 3] < 128 ? 255 : (d[p] * 77 + d[p + 1] * 151 + d[p + 2] * 28) >> 8;
      /* local mean threshold through an integral image */
      var W1 = w + 1, integ = new Float64Array(W1 * (h + 1)), bin = new Uint8Array(w * h), rs, half = Math.max(8, Math.round(Math.max(w, h) / 12));
      for (y2 = 0; y2 < h; y2++) { rs = 0; for (x2 = 0; x2 < w; x2++) { rs += gray[y2 * w + x2]; integ[(y2 + 1) * W1 + x2 + 1] = integ[y2 * W1 + x2 + 1] + rs; } }
      var lo = 255, hi = 0; for (n = 0; n < w * h; n += 7) { if (gray[n] < lo) lo = gray[n]; if (gray[n] > hi) hi = gray[n]; }
      if (hi - lo < 40) return null;
      for (y2 = 0; y2 < h; y2++) for (x2 = 0; x2 < w; x2++) {
        var x0 = Math.max(0, x2 - half), x1 = Math.min(w, x2 + half + 1), y0 = Math.max(0, y2 - half), y1 = Math.min(h, y2 + half + 1);
        var mean = (integ[y1 * W1 + x1] - integ[y0 * W1 + x1] - integ[y1 * W1 + x0] + integ[y0 * W1 + x0]) / ((x1 - x0) * (y1 - y0)), g0 = gray[y2 * w + x2];
        bin[y2 * w + x2] = (g0 < mean - 8 || (g0 < mean + 8 && g0 < (lo + hi) / 2 && mean < (lo + hi) / 2)) ? 1 : 0;
      }
      function B(xx, yy) { xx = Math.round(xx); yy = Math.round(yy); return xx < 0 || yy < 0 || xx >= w || yy >= h ? 0 : bin[yy * w + xx]; }
      function ratio(c) { var tot = c[0] + c[1] + c[2] + c[3] + c[4], ms, tol; if (tot < 7) return 0; ms = tot / 7; tol = ms * 0.7; return Math.abs(c[0] - ms) < tol && Math.abs(c[1] - ms) < tol && Math.abs(c[2] - 3 * ms) < 3 * tol * 0.6 && Math.abs(c[3] - ms) < tol && Math.abs(c[4] - ms) < tol ? ms : 0; }
      /* run check through (cx,cy) along (ux,uy): returns [center offset, module size] or null */
      function cross(cx, cy, ux, uy, maxLen) {
        var c = [0, 0, 0, 0, 0], a = 0, b2 = 0;
        if (!B(cx, cy)) return null;
        while (a < maxLen && B(cx - ux * (a + 1), cy - uy * (a + 1))) a++; c[2] = a; var a1 = a;
        while (a < maxLen * 2 && !B(cx - ux * (a + 1), cy - uy * (a + 1))) a++; c[1] = a - a1; var a2 = a;
        while (a < maxLen * 3 && B(cx - ux * (a + 1), cy - uy * (a + 1))) a++; c[0] = a - a2;
        while (b2 < maxLen && B(cx + ux * (b2 + 1), cy + uy * (b2 + 1))) b2++; c[2] += b2 + 1; var b1 = b2;
        while (b2 < maxLen * 2 && !B(cx + ux * (b2 + 1), cy + uy * (b2 + 1))) b2++; c[3] = b2 - b1; var b3 = b2;
        while (b2 < maxLen * 3 && B(cx + ux * (b2 + 1), cy + uy * (b2 + 1))) b2++; c[4] = b2 - b3;
        var ms = ratio(c); if (!ms) return null;
        return [(b1 - a1) / 2, ms];
      }
      var found = [], st = h > 600 ? 2 : 1, c5, runs, col, xs;
      function add(cx, cy, ms) { for (var q = 0; q < found.length; q++) { var F2 = found[q]; if (Math.abs(F2.x - cx) < F2.ms * 3.5 && Math.abs(F2.y - cy) < F2.ms * 3.5) { F2.x = (F2.x * F2.n + cx) / (F2.n + 1); F2.y = (F2.y * F2.n + cy) / (F2.n + 1); F2.ms = (F2.ms * F2.n + ms) / (F2.n + 1); F2.n++; return; } } found.push({ x: cx, y: cy, ms: ms, n: 1 }); }
      for (y2 = 0; y2 < h; y2 += st) {
        runs = []; col = bin[y2 * w]; xs = 0;
        for (x2 = 1; x2 <= w; x2++) if (x2 === w || bin[y2 * w + x2] !== col) { runs.push([col, xs, x2 - xs]); xs = x2; col = x2 < w ? bin[y2 * w + x2] : 0; }
        for (n = 0; n + 4 < runs.length; n++) {
          if (!runs[n][0]) continue;
          c5 = [runs[n][2], runs[n + 1][2], runs[n + 2][2], runs[n + 3][2], runs[n + 4][2]];
          var ms0 = ratio(c5); if (!ms0) continue;
          var cx = runs[n + 2][1] + runs[n + 2][2] / 2, vv = cross(cx, y2, 0, 1, ms0 * 5); if (!vv) continue;
          var cy = y2 + vv[0], hh2 = cross(cx, cy, 1, 0, ms0 * 5); if (!hh2) continue;
          cx += hh2[0];
          var dg = cross(cx, cy, 0.7071, 0.7071, ms0 * 5); if (!dg) continue;
          add(cx, cy, (vv[1] + hh2[1]) / 2);
        }
      }
      found = found.filter(function (F2) { return F2.n >= 2; });
      if (found.length < 3) return null;
      found.sort(function (a, b2) { return b2.n - a.n; }); found = found.slice(0, 8);
      var triples = [], a, b3, c;
      function dd(P, Q) { return Math.sqrt((P.x - Q.x) * (P.x - Q.x) + (P.y - Q.y) * (P.y - Q.y)); }
      for (a = 0; a < found.length; a++) for (b3 = a + 1; b3 < found.length; b3++) for (c = b3 + 1; c < found.length; c++) {
        var P = [found[a], found[b3], found[c]], ds = [[dd(P[1], P[2]), 0], [dd(P[0], P[2]), 1], [dd(P[0], P[1]), 2]].sort(function (m1, m2) { return m2[0] - m1[0]; });
        var tl = P[ds[0][1]], o1 = P[ds[1][1]], o2 = P[ds[2][1]], s1 = dd(tl, o1), s2 = dd(tl, o2);
        var err = Math.abs(s1 - s2) / Math.max(s1, s2) + Math.abs(ds[0][0] - Math.sqrt(s1 * s1 + s2 * s2)) / ds[0][0] + Math.abs(tl.ms - o1.ms) / tl.ms + Math.abs(tl.ms - o2.ms) / tl.ms;
        if (err < 0.9) triples.push({ e: err, tl: tl, a: o1, b: o2 });
      }
      triples.sort(function (m1, m2) { return m1.e - m2.e; });
      for (n = 0; n < triples.length && n < 4; n++) {
        var T3 = triples[n], TL = T3.tl, TR = T3.a, BL = T3.b, sw;
        if ((TR.x - TL.x) * (BL.y - TL.y) - (TR.y - TL.y) * (BL.x - TL.x) < 0) { sw = TR; TR = BL; BL = sw; }
        var ms2 = (TL.ms + TR.ms + BL.ms) / 3, est = ((dd(TL, TR) + dd(TL, BL)) / 2) / ms2 + 7, v0 = Math.round((est - 17) / 4), tryV = [v0, v0 + 1, v0 - 1, v0 + 2, v0 - 2], q, res;
        for (q = 0; q < tryV.length; q++) {
          if (tryV[q] < 1 || tryV[q] > 40) continue;
          res = sample(TL, TR, BL, tryV[q] * 4 + 17);
          if (res) return res;
        }
      }
      return null;
      function sample(TL, TR, BL, dim) {
        var span = dim - 7, br = [TR.x + BL.x - TL.x, TR.y + BL.y - TL.y], attempts = [], k2, tf, mod, ry, rx, pt, r2;
        function aff(mx, my) { var u = (mx - 3.5) / span, v2 = (my - 3.5) / span; return [TL.x + u * (TR.x - TL.x) + v2 * (BL.x - TL.x), TL.y + u * (TR.y - TL.y) + v2 * (BL.y - TL.y)]; }
        if (dim > 21) {
          var ex = aff(dim - 6.5, dim - 6.5), ux = (TR.x - TL.x) / span, uy = (TR.y - TL.y) / span, vx = (BL.x - TL.x) / span, vy = (BL.y - TL.y) / span, bestS = 0, bestPt = null, sx2, sy2, sc, i2, j2, rad = Math.max(4, Math.min(12, span / 4)), step = 0.5;
          for (sy2 = -rad; sy2 <= rad; sy2 += step) for (sx2 = -rad; sx2 <= rad; sx2 += step) {
            var ox = ex[0] + sx2 * ux + sy2 * vx, oy = ex[1] + sx2 * uy + sy2 * vy; sc = 0;
            if (!B(ox, oy)) continue;
            for (j2 = -2; j2 <= 2; j2++) for (i2 = -2; i2 <= 2; i2++) { var want = Math.max(Math.abs(i2), Math.abs(j2)) !== 1 ? 1 : 0; if (B(ox + i2 * ux + j2 * vx, oy + i2 * uy + j2 * vy) === want) sc++; }
            sc -= (Math.abs(sx2) + Math.abs(sy2)) * 0.05;
            if (sc > bestS) { bestS = sc; bestPt = [ox, oy]; }
          }
          if (bestPt && bestS >= 22) {
            /* centre the hit on its dark middle module */
            var cxa = cross2(bestPt[0], bestPt[1], ux, uy), cya;
            bestPt = [bestPt[0] + cxa * ux, bestPt[1] + cxa * uy]; cya = cross2(bestPt[0], bestPt[1], vx, vy); bestPt = [bestPt[0] + cya * vx, bestPt[1] + cya * vy];
            tf = homography([[3.5, 3.5], [dim - 3.5, 3.5], [3.5, dim - 3.5], [dim - 6.5, dim - 6.5]], [[TL.x, TL.y], [TR.x, TR.y], [BL.x, BL.y], bestPt]);
            if (tf) attempts.push(tf);
          }
        }
        attempts.push(aff);
        for (k2 = 0; k2 < attempts.length; k2++) {
          mod = [];
          for (ry = 0; ry < dim; ry++) { var row = new Uint8Array(dim); for (rx = 0; rx < dim; rx++) { pt = attempts[k2](rx + 0.5, ry + 0.5); row[rx] = B(pt[0], pt[1]); } mod.push(row); }
          r2 = decode(mod);
          if (r2) return r2;
        }
        return null;
      }
      function cross2(px, py, ux, uy) { var a2 = 0, b4 = 0, len = Math.sqrt(ux * ux + uy * uy), sx3 = ux / len, sy3 = uy / len; if (!B(px, py)) return 0; while (a2 < len * 2 && B(px - sx3 * (a2 + 1), py - sy3 * (a2 + 1))) a2++; while (b4 < len * 2 && B(px + sx3 * (b4 + 1), py + sy3 * (b4 + 1))) b4++; return (b4 - a2) / 2 / len; }
    }
    /* draw on a canvas; returns the canvas. o: size(px), margin(modules), dark, light, shape:'square'|'dot'|'round' */
    function draw(cv, q, o) {
      o = o || {};
      var mg = o.margin == null ? 4 : Math.max(0, Math.round(o.margin)), n = q.size + mg * 2, px = Math.max(1, Math.floor((o.size || 512) / n)), S = px * n, ctx, yy, xx, shape = o.shape || 'square';
      cv.width = S; cv.height = S; ctx = cv.getContext('2d');
      ctx.fillStyle = o.light || '#FFFFFF'; ctx.fillRect(0, 0, S, S); ctx.fillStyle = o.dark || '#000000';
      function isEye(x3, y3) { return (x3 < 7 && y3 < 7) || (x3 >= q.size - 7 && y3 < 7) || (x3 < 7 && y3 >= q.size - 7); }
      for (yy = 0; yy < q.size; yy++) for (xx = 0; xx < q.size; xx++) {
        if (!q.modules[yy][xx]) continue;
        var X = (xx + mg) * px, Y = (yy + mg) * px;
        if (shape === 'square' || isEye(xx, yy) || px < 4) ctx.fillRect(X, Y, px, px);
        else if (shape === 'dot') { ctx.beginPath(); ctx.arc(X + px / 2, Y + px / 2, px * 0.46, 0, Math.PI * 2); ctx.fill(); }
        else { var r = px * 0.32; ctx.beginPath(); ctx.moveTo(X + r, Y); ctx.arcTo(X + px, Y, X + px, Y + px, r); ctx.arcTo(X + px, Y + px, X, Y + px, r); ctx.arcTo(X, Y + px, X, Y, r); ctx.arcTo(X, Y, X + px, Y, r); ctx.fill(); }
      }
      return cv;
    }
    return { encode: encode, decode: decode, read: read, draw: draw, capacity: function (v, ecc) { var l = LV[ecc] == null ? 1 : LV[ecc]; return { codewords: dataCodewords(v, l), bytes: Math.floor((dataCodewords(v, l) * 8 - 4 - ccBits(4, v)) / 8) }; }, alignPos: alignPos, _rsFix: rsFix };
  })();


/* BYVE 본보기 공용(v3 11-26: 통화 125·나라 162·이름 16·양력 고정): 통화·예시 금액·예시 이름 (11-26 운영 로캘 사고 고침). 앱 공용 코드 맨 앞에 그대로 넣어 쓴다.
   우선순위: window.BYVE_CURRENCY(요청에 통화·나라가 적혔을 때 고치기 모델이 앱 맨 위에 한 줄로 씀) > window.__BYVE_LOC(서버가 넣음 {lang,region,currency}) > navigator.language 의 지역(ar-EG → EGP) > <html lang> 기본 통화 > USD.
   한국어(ko) 또는 KRW 이면 배율 1 → 지금 화면과 똑같다. */
var LOC = (function () {
  // 통화: 기호, 기호 자리(pre/post), 소수 자리, 원화 1원당 값(대략, 예시 크기용)
  var C = {
    KRW: ['₩', 'pre', 0, 1], USD: ['$', 'pre', 2, 1 / 1350], EUR: ['€', 'post', 2, 1 / 1450], GBP: ['£', 'pre', 2, 1 / 1700],
    JPY: ['¥', 'pre', 0, 0.11], CNY: ['¥', 'pre', 2, 1 / 190], TWD: ['NT$', 'pre', 0, 1 / 43], HKD: ['HK$', 'pre', 2, 1 / 175],
    IDR: ['Rp', 'pre', 0, 11.5], VND: ['₫', 'post', 0, 18], THB: ['฿', 'pre', 0, 1 / 39], PHP: ['₱', 'pre', 2, 1 / 24], MYR: ['RM', 'pre', 2, 1 / 300],
    INR: ['₹', 'pre', 0, 1 / 16], PKR: ['Rs', 'pre', 0, 0.2], BDT: ['৳', 'pre', 0, 1 / 11.5],
    SAR: ['ر.س', 'post', 2, 1 / 360], AED: ['د.إ', 'post', 2, 1 / 370], EGP: ['ج.م', 'post', 0, 1 / 28], IQD: ['د.ع', 'post', 0, 0.95],
    MAD: ['د.م.', 'post', 2, 1 / 140], DZD: ['د.ج', 'post', 0, 1 / 10], TND: ['د.ت', 'post', 2, 1 / 450], SDG: ['ج.س', 'post', 0, 0.44],
    JOD: ['د.أ', 'post', 2, 1 / 1900], KWD: ['د.ك', 'post', 3, 1 / 4400], QAR: ['ر.ق', 'post', 2, 1 / 370], LYD: ['د.ل', 'post', 2, 1 / 280],
    IRR: ['تومان', 'post', 0, 0.06], AFN: ['؋', 'post', 0, 1 / 19], TRY: ['₺', 'pre', 0, 1 / 41], RUB: ['₽', 'post', 0, 1 / 15],
    UAH: ['₴', 'post', 0, 1 / 33], KZT: ['₸', 'post', 0, 0.37], UZS: ['soʻm', 'post', 0, 9.3], AZN: ['₼', 'post', 2, 1 / 800],
    NGN: ['₦', 'pre', 0, 1.1], KES: ['KSh', 'pre', 0, 1 / 10.5], GHS: ['GH₵', 'pre', 2, 1 / 90], ZAR: ['R', 'pre', 2, 1 / 75],
    XOF: ['F CFA', 'post', 0, 0.42], XAF: ['F CFA', 'post', 0, 0.42], ETB: ['Br', 'post', 0, 1 / 11],
    BRL: ['R$', 'pre', 2, 1 / 250], MXN: ['$', 'pre', 2, 1 / 75], COP: ['$', 'pre', 0, 2.9], ARS: ['$', 'pre', 0, 0.75], CLP: ['$', 'pre', 0, 0.68], PEN: ['S/', 'pre', 2, 1 / 370],
    CAD: ['$', 'pre', 2, 1 / 1000], AUD: ['$', 'pre', 2, 1 / 900], CHF: ['CHF', 'pre', 2, 1 / 1600], PLN: ['zł', 'post', 2, 1 / 350],
    ZMW: ['K', 'pre', 2, 1 / 52], TZS: ['TSh', 'pre', 0, 1.85], UGX: ['USh', 'pre', 0, 2.7], RWF: ['FRw', 'pre', 0, 1.04], MWK: ['MK', 'pre', 0, 1.3], SOS: ['Sh', 'pre', 0, 0.42],
    CDF: ['FC', 'post', 0, 2.1], AOA: ['Kz', 'post', 0, 0.67], MZN: ['MT', 'post', 2, 1 / 21], BWP: ['P', 'pre', 2, 1 / 100], NAD: ['$', 'pre', 2, 1 / 75], ZWL: ['$', 'pre', 2, 1 / 1350],
    LKR: ['Rs', 'pre', 0, 0.22], NPR: ['Rs', 'pre', 0, 0.1], MMK: ['K', 'post', 0, 1.55], KHR: ['៛', 'post', 0, 3], LAK: ['₭', 'pre', 0, 15.5], MNT: ['₮', 'pre', 0, 2.5],
    SGD: ['$', 'pre', 2, 1 / 1040], NZD: ['$', 'pre', 2, 1 / 800], BND: ['$', 'pre', 2, 1 / 1040], MOP: ['MOP$', 'pre', 2, 1 / 170],
    GEL: ['₾', 'post', 2, 1 / 500], AMD: ['֏', 'post', 0, 0.29], BYN: ['Br', 'post', 2, 1 / 410], KGS: ['сом', 'post', 0, 1 / 15.5], TJS: ['SM', 'post', 2, 1 / 126], TMT: ['m', 'post', 2, 1 / 386],
    YER: ['ر.ي', 'post', 0, 0.185], SYP: ['ل.س', 'post', 0, 9.6], LBP: ['ل.ل', 'post', 0, 66], OMR: ['ر.ع', 'post', 3, 1 / 3500], BHD: ['د.ب', 'post', 3, 1 / 3590], ILS: ['₪', 'pre', 2, 1 / 365],
    MRU: ['UM', 'post', 0, 1 / 34], DJF: ['Fdj', 'post', 0, 0.13], KMF: ['CF', 'post', 0, 0.33], MGA: ['Ar', 'post', 0, 3.3], GNF: ['FG', 'post', 0, 6.4], SLE: ['Le', 'pre', 2, 1 / 60], LRD: ['$', 'pre', 2, 1 / 7],
    GMD: ['D', 'pre', 2, 1 / 19], CVE: ['$', 'post', 0, 1 / 13], SSP: ['£', 'pre', 0, 1 / 1.5], ERN: ['Nfk', 'pre', 0, 1 / 90],
    BOB: ['Bs', 'pre', 2, 1 / 196], PYG: ['₲', 'pre', 0, 5.8], UYU: ['$', 'pre', 0, 1 / 34], VES: ['Bs', 'pre', 2, 1 / 9], DOP: ['RD$', 'pre', 0, 1 / 22.5], GTQ: ['Q', 'pre', 2, 1 / 175],
    HNL: ['L', 'pre', 2, 1 / 54], NIO: ['C$', 'pre', 2, 1 / 37], CRC: ['₡', 'pre', 0, 0.37], PAB: ['B/.', 'pre', 2, 1 / 1350], CUP: ['$', 'pre', 0, 1 / 56], HTG: ['G', 'post', 0, 0.097], JMD: ['$', 'pre', 0, 0.116], TTD: ['$', 'pre', 2, 1 / 200],
    SEK: ['kr', 'post', 0, 1 / 129], NOK: ['kr', 'post', 0, 1 / 125], DKK: ['kr', 'post', 2, 1 / 199], CZK: ['Kč', 'post', 0, 1 / 59], HUF: ['Ft', 'post', 0, 0.27], RON: ['lei', 'post', 2, 1 / 293],
    BGN: ['лв', 'post', 2, 1 / 750], RSD: ['дин', 'post', 0, 1 / 12.7], MKD: ['ден', 'post', 0, 1 / 24], ALL: ['L', 'post', 0, 1 / 15], BAM: ['KM', 'post', 2, 1 / 740], MDL: ['L', 'post', 2, 1 / 76], ISK: ['kr', 'post', 0, 1 / 9.8]
  };
  // 지역 → 통화
  var R = { KR: 'KRW', US: 'USD', GB: 'GBP', JP: 'JPY', CN: 'CNY', TW: 'TWD', HK: 'HKD', ID: 'IDR', VN: 'VND', TH: 'THB', PH: 'PHP', MY: 'MYR', IN: 'INR', PK: 'PKR', BD: 'BDT',
    SA: 'SAR', AE: 'AED', EG: 'EGP', IQ: 'IQD', MA: 'MAD', DZ: 'DZD', TN: 'TND', SD: 'SDG', JO: 'JOD', KW: 'KWD', QA: 'QAR', LY: 'LYD', IR: 'IRR', AF: 'AFN', TR: 'TRY', RU: 'RUB',
    UA: 'UAH', KZ: 'KZT', UZ: 'UZS', AZ: 'AZN', NG: 'NGN', KE: 'KES', GH: 'GHS', ZA: 'ZAR', SN: 'XOF', CI: 'XOF', ML: 'XOF', BF: 'XOF', BJ: 'XOF', TG: 'XOF', NE: 'XOF', CM: 'XAF', GA: 'XAF', CG: 'XAF', TD: 'XAF', ET: 'ETB',
    BR: 'BRL', MX: 'MXN', CO: 'COP', AR: 'ARS', CL: 'CLP', PE: 'PEN', CA: 'CAD', AU: 'AUD', CH: 'CHF', PL: 'PLN', PT: 'EUR', ES: 'EUR', FR: 'EUR', DE: 'EUR', IT: 'EUR', NL: 'EUR', BE: 'EUR', AT: 'EUR', IE: 'EUR', GR: 'EUR', FI: 'EUR', ZM: 'ZMW', TZ: 'TZS', UG: 'UGX', RW: 'RWF', MW: 'MWK', SO: 'SOS', CD: 'CDF', AO: 'AOA', MZ: 'MZN', BW: 'BWP', NA: 'NAD', ZW: 'USD', LK: 'LKR', NP: 'NPR', MM: 'MMK', KH: 'KHR', LA: 'LAK', MN: 'MNT', SG: 'SGD', NZ: 'NZD', BN: 'BND', MO: 'MOP', GE: 'GEL', AM: 'AMD', BY: 'BYN', KG: 'KGS', TJ: 'TJS', TM: 'TMT', YE: 'YER', SY: 'SYP', LB: 'LBP', OM: 'OMR', BH: 'BHD', IL: 'ILS', PS: 'ILS', MR: 'MRU', DJ: 'DJF', KM: 'KMF', MG: 'MGA', GN: 'GNF', SL: 'SLE', LR: 'LRD', GM: 'GMD', CV: 'CVE', SS: 'SSP', ER: 'ERN', GW: 'XOF', GQ: 'XAF', CF: 'XAF', BO: 'BOB', PY: 'PYG', UY: 'UYU', VE: 'VES', DO: 'DOP', GT: 'GTQ', HN: 'HNL', NI: 'NIO', CR: 'CRC', PA: 'PAB', CU: 'CUP', HT: 'HTG', JM: 'JMD', TT: 'TTD', EC: 'USD', SV: 'USD', PR: 'USD', SE: 'SEK', NO: 'NOK', DK: 'DKK', CZ: 'CZK', HU: 'HUF', RO: 'RON', BG: 'BGN', RS: 'RSD', MK: 'MKD', AL: 'ALL', BA: 'BAM', MD: 'MDL', IS: 'ISK', LU: 'EUR', SK: 'EUR', SI: 'EUR', EE: 'EUR', LV: 'EUR', LT: 'EUR', HR: 'EUR', CY: 'EUR', MT: 'EUR', ME: 'EUR', XK: 'EUR' };
  // 언어만 알 때 기본 통화
  var L = { ko: 'KRW', en: 'USD', ja: 'JPY', zh: 'CNY', id: 'IDR', ms: 'MYR', vi: 'VND', th: 'THB', hi: 'INR', ur: 'PKR', bn: 'BDT', ar: 'SAR', fa: 'IRR', tr: 'TRY', ru: 'RUB', uk: 'UAH', kk: 'KZT', uz: 'UZS', az: 'AZN',
    fr: 'EUR', de: 'EUR', it: 'EUR', es: 'EUR', pt: 'BRL', nl: 'EUR', el: 'EUR', pl: 'PLN', sw: 'KES', ha: 'NGN', am: 'ETB', so: 'SOS', ps: 'AFN', ne: 'NPR', si: 'LKR', my: 'MMK', km: 'KHR', lo: 'LAK', mn: 'MNT', ka: 'GEL', hy: 'AMD', be: 'BYN', ky: 'KGS', tg: 'TJS', tk: 'TMT', he: 'ILS', sv: 'SEK', no: 'NOK', nb: 'NOK', da: 'DKK', cs: 'CZK', hu: 'HUF', ro: 'RON', bg: 'BGN', sr: 'RSD', mk: 'MKD', sq: 'ALL', is: 'ISK', rw: 'RWF', mg: 'MGA', fil: 'PHP', tl: 'PHP' };
  var g = (typeof window != 'undefined' && window.__BYVE_LOC) || {}, nav = (typeof navigator != 'undefined' && navigator.language) || '',
    lang = String(g.lang || (document.documentElement.getAttribute('lang')) || nav || 'ko').toLowerCase().split('-')[0],
    navLang = nav.toLowerCase().split('-')[0], region = String(g.region || (navLang === lang ? (nav.split('-')[1] || '') : '')).toUpperCase(),
    code = String((typeof window != 'undefined' && window.BYVE_CURRENCY) || g.currency || R[region] || L[lang] || 'USD').toUpperCase(), c = C[code] || [code, 'post', 2, C.USD[3]], rate = c[3];
  var NAMES = {
    en: ['Emma', 'Liam', 'Olivia', 'Noah', 'Ava', 'Lucas', 'Mia', 'Ethan', 'Sofia', 'Leo', 'Grace', 'Henry', 'Zoe', 'Isaac', 'Ruby', 'Owen'],
    ar: ['سارة', 'أحمد', 'مريم', 'يوسف', 'نور', 'عمر', 'ليلى', 'خالد', 'هدى', 'علي', 'فاطمة', 'حسن', 'زينب', 'محمد', 'رنا', 'سامي'],
    fa: ['سارا', 'علی', 'مریم', 'رضا', 'زهرا', 'امیر', 'نگار', 'حسین', 'نازنین', 'مهدی', 'فاطمه', 'محمد', 'الهام', 'کاوه', 'شیرین', 'بهرام'],
    fr: ['Camille', 'Lucas', 'Léa', 'Hugo', 'Chloé', 'Louis', 'Inès', 'Jules', 'Manon', 'Adam', 'Emma', 'Nathan', 'Zoé', 'Théo', 'Louise', 'Raphaël'],
    es: ['Lucía', 'Mateo', 'Sofía', 'Diego', 'Valentina', 'Santiago', 'Camila', 'Javier', 'Elena', 'Pablo', 'Martina', 'Hugo', 'Paula', 'Daniel', 'Carmen', 'Andrés'],
    pt: ['Ana', 'João', 'Beatriz', 'Pedro', 'Mariana', 'Lucas', 'Júlia', 'Gabriel', 'Larissa', 'Rafael', 'Fernanda', 'Thiago', 'Camila', 'Felipe', 'Letícia', 'Bruno'],
    id: ['Siti', 'Budi', 'Dewi', 'Agus', 'Putri', 'Rizky', 'Ayu', 'Andi', 'Nur', 'Dimas', 'Indah', 'Fajar', 'Ratna', 'Hendra', 'Wulan', 'Yusuf'],
    ru: ['Анна', 'Иван', 'Мария', 'Дмитрий', 'Елена', 'Алексей', 'Ольга', 'Сергей', 'Наталья', 'Павел', 'Татьяна', 'Андрей', 'Ирина', 'Николай', 'Светлана', 'Михаил'],
    tr: ['Elif', 'Mehmet', 'Zeynep', 'Mustafa', 'Ayşe', 'Emre', 'Fatma', 'Can', 'Merve', 'Burak', 'Selin', 'Ahmet', 'Ece', 'Murat', 'Deniz', 'Kerem'],
    de: ['Lena', 'Lukas', 'Anna', 'Felix', 'Marie', 'Jonas', 'Sophie', 'Paul', 'Laura', 'Ben', 'Mia', 'Leon', 'Emma', 'Noah', 'Hannah', 'Elias'],
    it: ['Giulia', 'Marco', 'Sofia', 'Luca', 'Chiara', 'Matteo', 'Sara', 'Andrea', 'Elena', 'Davide', 'Alice', 'Lorenzo', 'Aurora', 'Giuseppe', 'Martina', 'Simone'],
    ja: ['さくら', '蓮', '陽菜', '大翔', '結衣', '湊', '美咲', '悠真', '葵', '颯太', '花子', '翔', '彩', '健太', '真央', '拓海'],
    zh: ['王芳', '李伟', '张静', '刘洋', '陈敏', '杨磊', '赵丽', '黄强', '周婷', '吴杰', '林娜', '孙浩', '徐敏', '马超', '何欣', '郭鹏'],
    vi: ['Lan', 'Minh', 'Hoa', 'Tuấn', 'Mai', 'Hùng', 'Linh', 'Nam', 'Trang', 'Đức', 'Hương', 'Quang', 'Thảo', 'Phong', 'Ngọc', 'Long'],
    hi: ['प्रिया', 'राहुल', 'अनीता', 'अमित', 'पूजा', 'विकास', 'नेहा', 'रोहित', 'सीमा', 'अर्जुन', 'कविता', 'सुरेश', 'दीपिका', 'मनोज', 'रिया', 'आदित्य'],
    th: ['มาลี', 'สมชาย', 'นภา', 'วิชัย', 'ปราณี', 'อนุชา', 'สุดา', 'ธนา', 'อรุณ', 'กมล', 'จันทร์', 'ประเสริฐ', 'ศิริ', 'วีระ', 'พร', 'ชัย']
  };
  function gl(l) { // BCP47 에 -u-ca-gregory 붙이기(이미 -u- 확장이 있으면 ca 만 더하기, ca 가 있으면 gregory 로)
    l = String(l); if (/-u-/.test(l)) return /-ca-[a-z0-9]+/.test(l) ? l.replace(/-ca-[a-z0-9]+/, '-ca-gregory') : l.replace('-u-', '-u-ca-gregory-');
    return l + '-u-ca-gregory';
  }
  function nice(v) { // 예시 금액을 그 통화에서 자연스러운 숫자로(유효 숫자 2자리, 작은 값은 .5/.99 없이)
    if (!v) return 0; var s = v < 0 ? -1 : 1, a = Math.abs(v), p = Math.pow(10, Math.max(0, Math.floor(Math.log10(a)) - 1)), r = Math.round(a / p) * p;
    if (c[2] && r < 20) r = Math.round(a * 2) / 2; return s * r;
  }
  return {
    lang: lang, region: region, code: code, sym: c[0], pos: c[1], digits: c[2], rate: rate, ko: lang === 'ko',
    tag: String(g.locale || (lang + (region ? '-' + region : ''))).split('-u-')[0], // 말(음성) 언어 등 확장 없는 BCP47
    locale: gl(g.locale || (lang + (region ? '-' + region : ''))), // 달력은 늘 양력(ar-SA 이슬람력·fa 페르시아력·th 불기 어긋남 방지)
    amt: function (krw) { return code === 'KRW' || g.native ? krw : nice(krw * rate); },            // 예시 금액: 원화 기준 숫자를 넣으면 그 통화 크기로
    money: function (n, d) { var x = Math.abs(n), dd = d != null ? d : (Math.round(x) === x ? 0 : c[2]), s;
      try { s = new Intl.NumberFormat(this.locale, { minimumFractionDigits: dd, maximumFractionDigits: dd }).format(x); } catch (e) { s = String(x); }
      s = c[1] === 'post' ? s + ' ' + c[0] : c[0] + s; return (n < 0 ? '−' : '') + s; },
    names: function (ko) { var t = NAMES[lang] || NAMES[{ ur: 'ar', ps: 'fa', ms: 'id' }[lang]] || NAMES.en; return lang === 'ko' ? ko : ko.map(function (_, i) { return t[i % t.length]; }); }, // 예시 사람 이름: ko 배열을 주면 그 언어 이름으로 같은 수만큼
    pick: function (table) { return table[lang] || table[{ fa: 'ar', ur: 'ar' }[lang]] || table.en || table.ko; } // 언어별 예시(이름 등) 고르기
  };
})();

/* ===== CORE: 저장 · 문구(T) · 시트 · 토스트 · 예시 자료 띠 · 날짜 · 아이콘. 앱 고유 코드는 "APP" 표시 아래부터 ===== */
const $=(s,r)=>(r||document).querySelector(s), $$=(s,r)=>[].slice.call((r||document).querySelectorAll(s));
const esc=s=>String(s==null?'':s).replace(/[&<>"']/g,c=>({'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;',"'":'&#39;'}[c]));
const uid=()=>Date.now().toString(36)+Math.random().toString(36).slice(2,6);
const pad=n=>(n<10?'0':'')+n, clamp=(v,a,b)=>Math.max(a,Math.min(b,v)), n1=v=>Math.round(v*10)/10;

/* 저장: localStorage, 막히면 메모리. 한 앱은 키 하나(KEY)에 자료 D 전체를 넣어요 */
const Store=(()=>{const mem={};let ok=true;try{localStorage.setItem('_t','1');localStorage.removeItem('_t')}catch(e){ok=false}
  return{get(k,dv){try{const v=ok?localStorage.getItem(k):mem[k];return v==null?dv:JSON.parse(v)}catch(e){return dv}},
         set(k,v){const s=JSON.stringify(v);try{if(ok)localStorage.setItem(k,s);else mem[k]=s}catch(e){mem[k]=s}}}})();

/* 문구: 화면에 보이는 글은 전부 T 한 곳(언어별 사전 LANGS)에서만 가져와요. 언어를 바꿀 땐 사전만 바꾸면 돼요 */
const CORE_T={
  ko:{close:'Close',undo:'Undo',cancel:'Cancel',save:'Save',del:'Delete',edit:'Edit',add:'Add',done:'Done',sample:'Sample data',clearSample:'Clear samples',sampleCleared:'Sample cleared',
      hm:'{h} hr {m} min',h:'{h} hr',m:'{m} min',md:'{m}/{d}',wd:['Sun','Mon','Tue','Wed','Thu','Fri','Sat'],deleted:'Deleted',saved:'Saved',needName:'Enter a name',copied:'Copied',copyFail:'Couldn\'t copy',noHost:'Works in the BYVE AI app'},
  en:{close:'Close',undo:'Undo',cancel:'Cancel',save:'Save',del:'Delete',edit:'Edit',add:'Add',done:'Done',sample:'Sample data',clearSample:'Clear samples',sampleCleared:'Samples cleared',
      hm:'{h}h {m}m',h:'{h}h',m:'{m}m',md:'{m}/{d}',wd:['Sun','Mon','Tue','Wed','Thu','Fri','Sat'],deleted:'Deleted',saved:'Saved',needName:'Please enter a name',copied:'Copied',copyFail:'Could not copy',noHost:'Works inside the BYVE AI app'}};
let T={};
function pickLang(L,def){const q=((location.search.match(/[?&]lang=([a-zA-Z-]+)/)||[])[1]||navigator.language||def).slice(0,2).toLowerCase();
  const l=L[q]?q:def, base=Object.assign({},CORE_T[CORE_T[l]?l:'en'],L[def],L[l]);
  document.documentElement.lang=l;document.documentElement.dir=base._rtl?'rtl':'ltr';return base}
const t=(k,v)=>{let s=T[k];if(s==null)return k;if(v&&typeof s==='string')s=s.replace(/\{(\w+)\}/g,(m,a)=>v[a]!=null?v[a]:m);return s};
const fmtMin=m=>{m=Math.round(m);const h=Math.floor(m/60),r=m%60;return h&&r?t('hm',{h,m:r}):h?t('h',{h}):t('m',{m:r})};
const fmtClock=s=>{s=Math.max(0,Math.round(s));return(s>=3600?Math.floor(s/3600)+':':'')+pad(Math.floor(s%3600/60))+':'+pad(s%60)};

/* 아이콘(선 아이콘 24): 앱이 쓰는 것만 빌드가 ICONS 에 넣어요 */
const ic=(n,s,w)=>{const b=ICONS[n];if(!b)return'';s=s||24;return`<svg class="ic${/^(chev|arrow)-[lr]$/.test(n)?' flip':''}" viewBox="0 0 24 24" width="${s}" height="${s}" fill="none" stroke="currentColor" stroke-width="${w||1.8}" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true">${b}</svg>`};

/* 날짜: 'YYYY-MM-DD' 글자로 다뤄요 */
const dkey=d=>d.getFullYear()+'-'+pad(d.getMonth()+1)+'-'+pad(d.getDate());
const pkey=k=>{const a=k.split('-');return new Date(+a[0],+a[1]-1,+a[2])};
const today=()=>dkey(new Date());
const wdOf=k=>pkey(k).getDay();               /* 0=일 */
const daysBetween=(a,b)=>Math.round((pkey(b)-pkey(a))/864e5);

/* 층(시트·전체 화면)과 안드로이드 뒤로 가기: 열 때 history 한 칸, 뒤로 가면 맨 위 층만 닫아요 */
const Layers=[];let pend=0,wait=[];
function hist(l){try{history.pushState({L:1},'');l.hs=true}catch(e){}}
function pushLayer(fn){const l={fn,hs:false};Layers.push(l);if(pend)wait.push(l);else hist(l);return l}
function popLayer(){const l=Layers.pop();if(!l)return;l.fn();if(l.hs){pend++;history.back()}else{const i=wait.indexOf(l);if(i>-1)wait.splice(i,1)}}
function closeLayer(l){const i=Layers.indexOf(l);if(i<0)return;if(i===Layers.length-1)popLayer();else{Layers.splice(i,1);l.fn()}}
addEventListener('popstate',()=>{if(pend){pend--;if(!pend)wait.splice(0).forEach(hist);return}const l=Layers.pop();if(l)l.fn()});
addEventListener('keydown',e=>{if(e.key==='Escape')popLayer()});
if(window.visualViewport){const f=()=>document.documentElement.style.setProperty('--vh',visualViewport.height+'px');visualViewport.addEventListener('resize',f);f()}

/* 시트: sheet({title, body(HTML), ok(단추 이름), onOk(api)→false 면 안 닫음, extra:[{label,cls,on(api)}], onOpen(api), onClose()}) */
function sheet(o){
  const ov=document.createElement('div');ov.className='ov';
  const foot=(o.ok||(o.extra&&o.extra.length))?`<div class="sh-f">${(o.extra||[]).map((x,i)=>`<button class="btn ${x.cls||''}" data-ex="${i}">${esc(x.label)}</button>`).join('')}${o.ok?`<button class="btn pri" data-ok>${esc(o.ok)}</button>`:''}</div>`:'';
  ov.innerHTML=`<div class="sh ${o.cls||''}" role="dialog" aria-modal="true"><div class="sh-h"><b>${esc(o.title||'')}</b><button class="sh-x" data-sx aria-label="${esc(t('close'))}">${ic('x',22)}</button></div><div class="sh-b">${o.body||''}</div>${foot}</div>`;
  document.body.appendChild(ov);
  let done=false;const api={el:ov,body:$('.sh-b',ov)};
  const layer=pushLayer(()=>{if(done)return;done=true;ov.classList.remove('on');setTimeout(()=>ov.remove(),280);if(o.onClose)o.onClose()});
  api.close=()=>closeLayer(layer);
  ov.addEventListener('click',e=>{
    if(e.target===ov||e.target.closest('[data-sx]')){api.close();return}
    const ex=e.target.closest('[data-ex]');if(ex){const x=o.extra[+ex.getAttribute('data-ex')];if(x.on(api)!==false)api.close();return}
    if(e.target.closest('[data-ok]')){if(o.onOk&&o.onOk(api)===false)return;api.close()}});
  ov.addEventListener('focusin',e=>{if(/INPUT|TEXTAREA|SELECT/.test(e.target.tagName))setTimeout(()=>{try{e.target.scrollIntoView({block:'center',behavior:'smooth'})}catch(x){}},320)});
  requestAnimationFrame(()=>requestAnimationFrame(()=>ov.classList.add('on')));
  if(o.onOpen)o.onOpen(api);
  return api;
}
const val=(sel,root)=>{const e=$(sel,root||document);return e?e.value.trim():''};
/* 시트 안 고르기(세그먼트·칩·색): data-v 값을 읽어요 */
function bindPick(root,sel,cb){root.addEventListener('click',e=>{const b=e.target.closest(sel);if(!b||!root.contains(b))return;$$(sel,root).forEach(x=>x.classList.remove('on'));b.classList.add('on');if(cb)cb(b.getAttribute('data-v'),b)})}
const picked=(root,sel)=>{const b=$(sel+'.on',root);return b?b.getAttribute('data-v'):''};
/* 숫자 올리고 내리기: <div class="stp" data-min="1" data-max="90" data-step="5"><button data-d="-1">…</button><b>25</b><button data-d="1">…</button></div> */
function bindStep(root){root.addEventListener('click',e=>{const b=e.target.closest('.stp [data-d]');if(!b)return;const s=b.parentNode,n=s.querySelector('b'),st=+(s.getAttribute('data-step')||1);n.textContent=clamp((+n.textContent||0)+st*(+b.getAttribute('data-d')),+(s.getAttribute('data-min')||0),+(s.getAttribute('data-max')||999))})}
const stepVal=(root,sel)=>+$(sel+' b',root).textContent;

/* 토스트(되돌리기 단추 포함) */
let toastT;
function toast(msg,o){o=o||{};let el=$('#toast');if(!el){el=document.createElement('div');el.id='toast';el.className='toast';document.body.appendChild(el)}
  el.innerHTML=`<span>${esc(msg)}</span>${o.undo?`<button data-undo>${esc(t('undo'))}</button>`:''}`;
  requestAnimationFrame(()=>el.classList.add('on'));clearTimeout(toastT);toastT=setTimeout(()=>el.classList.remove('on'),o.undo?5000:2200);
  el.onclick=e=>{if(e.target.closest('[data-undo]')){clearTimeout(toastT);el.classList.remove('on');o.undo()}}}

/* 예시 자료: 처음 한 번만 넣고(항목에 s:1), 남아 있는 동안 화면 맨 위 흐름 안에 "Clear sample" 띠를 둬요. 사용자가 고친 항목은 s 를 지워요 */
const seedHas=o=>{for(const k in o){const v=o[k];if(Array.isArray(v)){for(let i=0;i<v.length;i++){const x=v[i];if(x&&typeof x==='object'&&(x.s||seedHas(x)))return true}}else if(v&&typeof v==='object'&&seedHas(v))return true}return false};
const seedClear=o=>{for(const k in o){const v=o[k];if(Array.isArray(v)){o[k]=v.filter(x=>!(x&&x.s));o[k].forEach(x=>{if(x&&typeof x==='object')seedClear(x)})}else if(v&&typeof v==='object')seedClear(v)}};
const seedBar=()=>seedHas(D)?`<div class="seedbar" role="note"><span>${esc(t('sample'))}</span><button data-a="clearSeed">${esc(t('clearSample'))}</button></div>`:'';
const own=x=>{if(x)delete x.s;return x};

/* 기기 기능(진동·화면 켜 두기 등)은 BYVE 가 있을 때만, 거절돼도 조용히 넘어가요 */
function host(name,args){try{if(window.BYVE&&BYVE.invoke){const p=BYVE.invoke(name,args||{});if(p&&p.catch)p.catch(()=>{});return p}}catch(e){}}

/* 호스트 호출을 약속(Promise)으로: 호스트가 없으면 no_host 로 거절, {data} 는 벗겨서 돌려줘요 */
const HAS=()=>!!(window.BYVE&&typeof BYVE.invoke==='function');
const errCode=e=>String(e&&(e.code||e.error||e.message)||'error');
function hostP(name,args){if(!HAS())return Promise.reject({code:'no_host'});try{return Promise.resolve(BYVE.invoke(name,args||{})).then(r=>{if(r&&(r.ok===false||(r.error&&r.data===undefined)))throw(r.error&&typeof r.error==='object'?r.error:{code:String(r.error||'failed')});return r&&r.data!==undefined?r.data:r})}catch(e){return Promise.reject(e)}}

/* 누름 위임: <button data-a="Name" data-id="..."> → ACT.이름(el,ev) */
const ACT={clearSeed(){seedClear(D);save();toast(t('sampleCleared'));render(true)}};
document.addEventListener('click',e=>{const el=e.target.closest('[data-a]');if(!el||el.disabled)return;const f=ACT[el.getAttribute('data-a')];if(f)f(el,e)});
/* 아래 탭 그리기: items=[{id,icon,label}] */
const navHTML=(items,cur)=>items.map(x=>`<button class="nv${x.id===cur?' on':''}" data-a="tab" data-id="${x.id}" aria-label="${esc(x.label)}">${ic(x.icon,24,x.id===cur?2:1.8)}<i>${esc(x.label)}</i></button>`).join('');

/* BYVE: 값이 비어 있는 날짜·시간 칸 표시(data-e) — 값이 있는 칸과 글자색을 가르기 위함 */
(function(){var R=/^(date|time|datetime-local|month|week)$/;function f(e){if(e&&e.tagName==='INPUT'&&R.test(e.type)){if(e.value)e.removeAttribute('data-e');else e.setAttribute('data-e','1')}}function all(){var l=document.querySelectorAll('input[type=date],input[type=time],input[type=datetime-local],input[type=month],input[type=week]');for(var i=0;i<l.length;i++)f(l[i])}document.addEventListener('input',function(e){f(e.target)},true);document.addEventListener('change',function(e){f(e.target)},true);if(window.MutationObserver)new MutationObserver(all).observe(document.documentElement,{childList:true,subtree:true});setInterval(all,600);all()})();
/* ===== APP ===== */
const KEY='phone-card-wallet';
const LANGS={
ko:{nWal:'Card',nScan:'Scan',nMake:'Create',cards:'Card',cnt:'cards',cardsL:'WALLET',show:'View larger',tapShow:'Tap to enlarge',
 kQr:'QR',kC128:'Barcode',kEan:'EAN-13',kWifi:'Wi-Fi',
 cols:{black:'Black',orange:'Orange',white:'White',gray:'Gray',navy:'Navy',green:'Green'},
 bigT:'Scan',scanB:'Scan with camera',scanSub:'Scan a barcode or QR code and save it as a card.',rdVal:'Scanned value',rdSave:'Save as card',rdCopy:'Copy',rdOpen:'Open link',
 scanFail:'Couldn\'t scan',scanNone:'No value scanned',noHostScan:'Camera scanning works in the BYVE AI app',
 pic:'Scan QR from photo',picFail:'Couldn\'t find a QR code in the photo',typeIn:'Enter value manually',
 mT:'Create card',mName:'Name',mVal:'Value',mSsid:'Wi-Fi name',mPw:'Password',mSec:'Security',mCol:'Card color',mSave:'Add to card',mHint:'e.g. Gym access',
 vHintQ:'Any text, link, phone number, etc.',vHintC:'Letters, numbers, symbols',vHintE:'12 digits (last digit automatic)',
 eEan:'Enter 12 or 13 digits',eEanChk:'Check digit doesn\'t match',eC128:'Some characters can\'t be used in a barcode',eQr:'Value is too long',eEmpty:'Enter a value',
 edT:'Edit card',saved2:'Card added',
 bright:'Brightness increased',sec:{WPA:'WPA',WEP:'WEP',nopass:'None'},
 seed:['Gym access','Library card','Local grocery rewards','Home Wi-Fi','Movie coupon','Bus pass','Package locker']},
en:{nWal:'Cards',nScan:'Scan',nMake:'Create',cards:'Cards',cnt:'',cardsL:'WALLET',show:'Show big',tapShow:'Tap to show it big',
 kQr:'QR',kC128:'Barcode',kEan:'EAN-13',kWifi:'Wi-Fi',
 cols:{black:'Black',orange:'Orange',white:'White',gray:'Gray',navy:'Navy',green:'Green'},
 bigT:'Scan',scanB:'Scan with camera',scanSub:'Read a barcode or QR and save it as a card.',rdVal:'Value read',rdSave:'Save as card',rdCopy:'Copy',rdOpen:'Open link',
 scanFail:'Could not read it',scanNone:'Nothing was read',noHostScan:'Camera scanning works inside the BYVE AI app',
 pic:'Read QR from a photo',picFail:'No QR found in the photo',typeIn:'Type a value',
 mT:'Create a card',mName:'Name',mVal:'Value',mSsid:'Wi-Fi name',mPw:'Password',mSec:'Security',mCol:'Card color',mSave:'Add to wallet',mHint:'e.g. Gym entry',
 vHintQ:'Any text, link or phone number',vHintC:'Letters, digits, symbols',vHintE:'12 digits (the last digit is automatic)',
 eEan:'Enter 12 or 13 digits',eEanChk:'The last digit does not match',eC128:'Contains characters a barcode cannot hold',eQr:'The value is too long',eEmpty:'Enter a value',
 edT:'Edit card',saved2:'Card added',
 bright:'Brightness raised',sec:{WPA:'WPA',WEP:'WEP',nopass:'None'},
 seed:['Gym entry','Library card','Local market points','Home Wi-Fi','Movie coupon','Bus pass','Parcel locker']}
};
T=pickLang(LANGS,'ko');
const COL={black:['#0d0d0d','#ffffff'],orange:['#ff4d00','#ffffff'],white:['#fffefa','#0d0d0d'],gray:['#c9c6bb','#0d0d0d'],navy:['#1b2a6b','#ffffff'],green:['#0b6b4b','#ffffff']};
const C128=['212222','222122','222221','121223','121322','131222','122213','122312','132212','221213','221312','231212','112232','122132','122231','113222','123122','123221','223211','221132','221231','213212','223112','312131','311222','321122','321221','312212','322112','322211','212123','212321','232121','111323','131123','131321','112313','132113','132311','211313','231113','231311','112133','112331','132131','113123','113321','133121','313121','211331','231131','213113','213311','213131','311123','311321','331121','312113','312311','332111','314111','221411','431111','111224','111422','121124','121421','141122','141221','112214','112412','122114','122411','142112','142211','241211','221114','413111','241112','134111','111242','121142','121241','114212','124112','124211','411212','421112','421211','212141','214121','412121','111143','111341','131141','114113','114311','411113','411311','113141','114131','311141','411131','211412','211214','211232','2331112'];
const EL='0001101 0011001 0010011 0111101 0100011 0110001 0101111 0111011 0110111 0001011'.split(' '),EG='0100111 0110011 0011011 0100001 0011101 0111001 0000101 0010001 0001001 0010111'.split(' '),ER=EL.map(s=>s.replace(/[01]/g,c=>c==='0'?'1':'0')),EP='LLLLLL LLGLGG LLGGLG LLGGGL LGLLGG LGGLLG LGGGLL LGLGLG LGLGGL LGGLGL'.split(' ');
const eanChk=d=>{let s=0;for(let i=0;i<12;i++)s+=(+d[i])*(i%2?3:1);return(10-s%10)%10};
function svgRects(bars,W,H,x0,extra){let s='',x=x0;bars.forEach(b=>{if(b[0])s+=`<rect x="${x}" y="0" width="${b[1]}" height="${b[2]||H}"/>`;x+=b[1]});return s}
function c128Bars(text){const allD=/^\d+$/.test(text)&&text.length%2===0&&text.length>=4;let vals=[],start;if(allD){start=105;for(let i=0;i<text.length;i+=2)vals.push(+text.substr(i,2))}else{start=104;for(let i=0;i<text.length;i++){const c=text.charCodeAt(i);if(c<32||c>126)return null;vals.push(c-32)}}
  let sum=start;vals.forEach((v,i)=>sum+=v*(i+1));const seq=[start].concat(vals,[sum%103,106]),bars=[];seq.forEach(v=>{const p=C128[v];for(let i=0;i<p.length;i++)bars.push([i%2===0?1:0,+p[i]])});return bars}
function codeSvg(k,v,px){v=String(v||'');if(!v)return{err:'eEmpty'};
  if(k==='qr'){if(v.length>600)return{err:'eQr'};let q;try{q=QR.encode(v,{ecc:'M'})}catch(e){return{err:'eQr'}}const n=q.size,m=3,N=n+m*2;let r='';for(let y=0;y<n;y++){let x=0;while(x<n){if(q.modules[y][x]){let e=x;while(e<n&&q.modules[y][e])e++;r+=`<rect x="${x+m}" y="${y+m}" width="${e-x}" height="1"/>`;x=e}else x++}}
   return{svg:`<svg viewBox="0 0 ${N} ${N}" width="${px||200}" height="${px||200}" shape-rendering="crispEdges"><rect width="${N}" height="${N}" fill="#fff"/><g fill="#000">${r}</g></svg>`,txt:v}}
  if(k==='c128'){const b=c128Bars(v);if(!b)return{err:'eC128'};const q=10,W=b.reduce((a,x)=>a+x[1],0)+q*2;return{svg:`<svg viewBox="0 0 ${W} 60" width="${px||300}" height="${Math.round((px||300)*60/W)}" shape-rendering="crispEdges" preserveAspectRatio="none"><rect width="${W}" height="60" fill="#fff"/><g fill="#000">${svgRects(b,W,60,q)}</g></svg>`,txt:v}}
  if(k==='ean'){let d=v.replace(/\s/g,'');if(!/^\d{12,13}$/.test(d))return{err:'eEan'};if(d.length===13){if(+d[12]!==eanChk(d))return{err:'eEanChk'}}else d+=eanChk(d);
   const par=EP[+d[0]];let bits='101';for(let i=1;i<7;i++)bits+=(par[i-1]==='L'?EL:EG)[+d[i]];bits+='01010';for(let i=7;i<13;i++)bits+=ER[+d[i]];bits+='101';
   let r='';for(let i=0;i<bits.length;i++)if(bits[i]==='1'){const g=i<3||(i>=45&&i<50)||i>=92;r+=`<rect x="${i+11}" y="0" width="1" height="${g?66:60}"/>`}
   const W=95+22;let tx='';tx+=`<text x="4" y="68" font-size="9" text-anchor="middle">${d[0]}</text>`;for(let i=1;i<13;i++){const x=i<7?11+3+(i-1)*7+3.5:11+50+(i-7)*7+3.5;tx+=`<text x="${x}" y="68" font-size="9" text-anchor="middle">${d[i]}</text>`}
   return{svg:`<svg viewBox="0 0 ${W} 72" width="${px||300}" height="${Math.round((px||300)*72/W)}" shape-rendering="crispEdges"><rect width="${W}" height="72" fill="#fff"/><g fill="#000">${r}</g><g fill="#000" font-family="Menlo,Courier New,monospace">${tx}</g></svg>`,txt:d}}
  return{err:'eEmpty'}}
const kName=k=>t(k==='qr'?'kQr':k==='c128'?'kC128':'kEan');
const SD=[['qr','https://example.com/event','orange'],['qr','https://example.com/library','black'],['qr','https://example.com/rewards','white'],['qr','WIFI:T:WPA;S:Home-5G;P:maple2026;;','gray'],['qr','https://example.com/ticket','navy'],['qr','https://example.com/travel','green'],['qr','https://example.com/pickup','black']];
function seed(){const names=['Event QR','Library QR','Rewards QR','Home Wi-Fi QR','Ticket QR','Travel QR','Pickup QR'];return{cards:T.seed.map((n,i)=>{const a=SD[i]||['qr','CARD-0000','black'];return{id:'c'+i,n:names[i]||'Saved QR',k:a[0],v:a[1],c:a[2],s:1}}),sel:'c0'}}
let D=Store.get(KEY,null);if(!D){D=seed();Store.set(KEY,D)}
const save=()=>Store.set(KEY,D);
let tab=Store.get(KEY+':tab','wal'),CF={k:'qr',n:'',v:'',ssid:'',pw:'',sec:'WPA',c:'black'},RS=null;
const card=id=>D.cards.find(c=>c.id===id)||D.cards[0];
function panel(c,px){const r=codeSvg(c.k,c.v,px);return r.err?`<div class="pn"><div class="vl">${esc(t(r.err))}</div></div>`:`<div class="pn">${r.svg}<div class="vl">${esc(r.txt.length>34?r.txt.slice(0,32)+'…':r.txt)}</div></div>`}
function cardStyle(c){const p=COL[c.c]||COL.black;return`--cb:${p[0]};--ci:${p[1]}`}
function vWal(){const sel=card(D.sel),rest=D.cards.filter(c=>c.id!==sel.id);
  return`<div class="top">${seedBar()}</div><div class="hd"><div class="n"><b>${D.cards.length}</b><span><small>${esc(t('cardsL'))}</small>${esc(t('cards'))}${esc(t('cnt'))}</span></div><button class="pls" data-a="goMake" aria-label="${esc(t('mT'))}">${ic('plus',28,3)}</button></div>
  ${D.cards.length?`<div class="stk"><div class="cd big" style="${cardStyle(sel)}"><div class="tp"><span class="ty">${esc(kName(sel.k))}</span><span class="nm">${esc(sel.n)}</span><button class="ex" data-a="edC" data-id="${sel.id}" aria-label="${esc(t('edT'))}">${ic('edit',20,2.4)}</button></div>${panel(sel,sel.k==='qr'?150:300)}<div class="hint"><span>${esc(t('tapShow'))}</span><button data-a="showC" data-id="${sel.id}">${esc(t('show'))}</button></div></div>
  ${rest.map(c=>`<button class="cd sm pick" style="${cardStyle(c)}" data-a="pickC" data-id="${c.id}"><span class="tp"><span class="ty">${esc(kName(c.k))}</span><span class="nm">${esc(c.n)}</span></span></button>`).join('')}</div>`:`<div class="empty" style="padding-top:60px"><b>${esc(t('cards'))} 0</b><button class="btn pri" data-a="goMake" style="background:#ff4d00;color:#fff">${esc(t('mSave'))}</button></div>`}<div class="tail"></div>`}
ACT.pickC=el=>{D.sel=el.dataset.id;save();render();$('#page').scrollTop=0};
ACT.goMake=()=>{tab='make';Store.set(KEY+':tab',tab);render()};
ACT.showC=el=>openShow(card(el.dataset.id));
function openShow(c){const ov=document.createElement('div');ov.className='shw';const r=codeSvg(c.k,c.v,c.k==='qr'?360:380);let br=false;
  ov.innerHTML=`<div class="hh"><b>${esc(c.n)}</b><button data-x aria-label="${esc(t('close'))}">${ic('x',26,2.8)}</button></div><div class="cv">${r.err?`<div class="vl">${esc(t(r.err))}</div>`:r.svg}<div class="vl">${esc(r.txt||'')}</div><div class="st" id="bt"></div></div>`;
  document.body.appendChild(ov);
  hostP('screen.brightness',{level:1}).then(()=>{br=true;const b=$('#bt',ov);if(b)b.textContent=t('bright')}).catch(()=>{});hostP('keepScreenOn',{state:'on'}).catch(()=>{});
  const layer=pushLayer(()=>{ov.remove();if(br)hostP('screen.brightness',{reset:true}).catch(()=>{});hostP('keepScreenOn',{state:'off'}).catch(()=>{})});
  ov.addEventListener('click',e=>{if(e.target.closest('[data-x]'))closeLayer(layer)})}
function cSheet(id,pre){const x=id?card(id):Object.assign({n:'',k:'qr',v:'',c:'black'},pre||{});
  sheet({title:t(id?'edT':'mT'),ok:t('save'),extra:id?[{label:t('del'),cls:'dng',on:()=>{const i=D.cards.findIndex(a=>a.id===id),o=D.cards.splice(i,1)[0];if(D.sel===id&&D.cards.length)D.sel=D.cards[0].id;save();render(true);toast(t('deleted'),{undo:()=>{D.cards.splice(i,0,o);save();render(true)}})}}]:null,
   body:`<label class="fld"><span>${esc(t('mName'))}</span><input class="in" id="cn" value="${esc(x.n)}"></label>
   <div class="fld"><span>${esc(t('kQr'))} / ${esc(t('kC128'))} / ${esc(t('kEan'))}</span><div class="seg" id="ck">${['qr','c128','ean'].map(k=>`<button data-v="${k}" class="${x.k===k?'on':''}">${esc(kName(k))}</button>`).join('')}</div></div>
   <label class="fld"><span>${esc(t('mVal'))}</span><input class="in" id="cv" value="${esc(x.v)}" autocapitalize="off" autocomplete="off"></label>
   <div class="fld"><span>${esc(t('mCol'))}</span><div class="sws2" id="cc">${Object.keys(COL).map(k=>`<button style="--cb:${COL[k][0]}" data-v="${k}" class="${x.c===k?'on':''}" aria-label="${esc(t('cols')[k])}"></button>`).join('')}</div></div><div class="err" id="ce" hidden></div>`,
   onOpen:a=>{bindPick(a.body,'#ck button');bindPick(a.body,'#cc button')},
   onOk:a=>{const n=val('#cn',a.body),v=val('#cv',a.body),k=picked(a.body,'#ck button')||'qr',r=codeSvg(k,v);if(r.err){const e=$('#ce',a.body);e.textContent=t(r.err);e.hidden=false;return false}
    const o=id?x:{id:'c'+uid()};o.n=n||kName(k);o.k=k;o.v=k==='ean'?r.txt:v;o.c=picked(a.body,'#cc button')||'black';own(o);if(!id){D.cards.push(o);D.sel=o.id}save();render(true)}})}
ACT.edC=el=>cSheet(el.dataset.id);

const kindOf=(txt,fmt)=>{fmt=String(fmt||'').toUpperCase();if(/QR/.test(fmt))return'qr';if(/EAN_13|EAN13/.test(fmt))return'ean';if(/CODE_?128/.test(fmt))return'c128';if(/^\d{13}$/.test(txt))return'ean';if(/^[\x20-\x7e]+$/.test(txt)&&txt.length<=40&&!/^(https?:|WIFI:|tel:|mailto:)/i.test(txt))return'c128';return'qr'};
function vScan(){return`<div class="top">${seedBar()}</div><div class="big2">${esc(t('bigT'))}</div><p class="sub">${esc(t('scanSub'))}</p>
  <div class="scn"><div class="fr"><i></i><i></i><i></i><i></i></div><span class="ls"></span><button class="gb" data-a="doScan">${ic('camera',20,2.6)} ${esc(t('scanB'))}</button></div>
  <div class="alt"><button class="btn out" data-a="pickImg">${esc(t('pic'))}</button><button class="btn out" data-a="typeIn">${esc(t('typeIn'))}</button></div>
  ${RS?`<div class="rsl"><span>${esc(t('rdVal'))} · ${esc(kName(RS.k))}</span><b>${esc(RS.v)}</b><div class="bt"><button class="btn org" data-a="rsSave">${esc(t('rdSave'))}</button><button class="btn out" data-a="rsCopy">${esc(t('rdCopy'))}</button>${/^https?:\/\//i.test(RS.v)?`<button class="btn blk" data-a="rsOpen">${esc(t('rdOpen'))}</button>`:''}</div></div>`:''}<div class="tail"></div>`}
function gotRead(v,f){v=String(v||'').trim();if(!v){toast(t('scanNone'));return}RS={v,k:kindOf(v,f)};render(true)}
ACT.doScan=()=>{hostP('barcode.scan',{}).then(r=>{const v=r&&(r.text||r.value||r.rawValue||r.data||r.code);gotRead(typeof v==='object'?'':v,r&&(r.format||r.type))}).catch(e=>{const c=errCode(e);if(c==='no_host')toast(t('noHostScan'));else if(c!=='cancelled')toast(t('scanFail'))})};
ACT.pickImg=async()=>{try{const picked=await BYVE.invoke('file.pick',{kind:'image'});if(!picked||!picked.data||!picked.data.assetId)throw new Error('file.pick failed');const r=await BYVE.invoke('barcode.scan',{});if(!r||r.ok===false||r.error)throw new Error('barcode.scan failed');const data=r.data||r,v=data.text||data.value||data.rawValue||data.data||data.code;if(v)gotRead(typeof v==='object'?'':v,data.format||data.type);else toast(t('picFail'))}catch(e){toast(t('picFail'))}};
ACT.typeIn=()=>{tab='make';CF={k:'qr',n:'',v:'',ssid:'',pw:'',sec:'WPA',c:'black'};Store.set(KEY+':tab',tab);render()};
ACT.rsSave=()=>{const r=RS;RS=null;CF={k:r.k,n:'',v:r.v,ssid:'',pw:'',sec:'WPA',c:'black'};tab='make';Store.set(KEY+':tab',tab);render()};
ACT.rsCopy=()=>hostP('clipboard.write',{text:RS.v}).then(()=>toast(t('copied'))).catch(()=>{if(navigator.clipboard&&navigator.clipboard.writeText)navigator.clipboard.writeText(RS.v).then(()=>toast(t('copied')),()=>toast(t('copyFail')));else toast(t('copyFail'))});
ACT.rsOpen=()=>hostP('browser.open',{url:RS.v,target:'inApp'}).catch(()=>toast(t('noHost')));

const wifiStr=()=>{const e=s=>String(s).replace(/([\\;,:"])/g,'\\$1');return'WIFI:T:'+CF.sec+';S:'+e(CF.ssid)+(CF.sec==='nopass'?'':';P:'+e(CF.pw))+';;'};
const cfVal=()=>CF.k==='wifi'?(CF.ssid?wifiStr():''):CF.v;
const cfKind=()=>CF.k==='wifi'?'qr':CF.k;
function pvHTML(){const v=cfVal(),r=v?codeSvg(cfKind(),v,CF.k==='qr'||CF.k==='wifi'?170:300):{err:'eEmpty'};return r.err?`<div class="er">${esc(t(r.err))}</div>`:`${r.svg}<div class="vl">${esc(r.txt.length>34?r.txt.slice(0,32)+'…':r.txt)}</div>`}
function vMake(){const k=CF.k;
  return`<div class="top">${seedBar()}</div><div class="big2">${esc(t('mT'))}</div>
  <div class="cf"><div class="seg4" id="ks">${[['qr','kQr'],['wifi','kWifi'],['c128','kC128'],['ean','kEan']].map(x=>`<button data-a="cfk" data-id="${x[0]}" class="${k===x[0]?'on':''}">${esc(t(x[1]))}</button>`).join('')}</div>
  <span class="lb2">${esc(t('mName'))}</span><input class="in" id="fn" value="${esc(CF.n)}" placeholder="${esc(t('mHint'))}">
  ${k==='wifi'?`<span class="lb2">${esc(t('mSsid'))}</span><input class="in" id="fs" value="${esc(CF.ssid)}" autocapitalize="off" autocomplete="off"><span class="lb2">${esc(t('mPw'))}</span><input class="in" id="fp" value="${esc(CF.pw)}" autocapitalize="off" autocomplete="off"><span class="lb2">${esc(t('mSec'))}</span><div class="seg4">${['WPA','WEP','nopass'].map(s=>`<button data-a="cfs" data-id="${s}" class="${CF.sec===s?'on':''}">${esc(t('sec')[s])}</button>`).join('')}</div>`:`<span class="lb2">${esc(t('mVal'))}</span><input class="in" id="fv" value="${esc(CF.v)}" placeholder="${esc(t(k==='qr'?'vHintQ':k==='c128'?'vHintC':'vHintE'))}" autocapitalize="off" autocomplete="off" ${k==='ean'?'inputmode="numeric"':''}>`}
  <span class="lb2">${esc(t('mCol'))}</span><div class="sws2">${Object.keys(COL).map(c=>`<button style="--cb:${COL[c][0]}" data-a="cfc" data-id="${c}" class="${CF.c===c?'on':''}" aria-label="${esc(t('cols')[c])}"></button>`).join('')}</div>
  <div class="pv" id="pv">${pvHTML()}</div><button class="btn block" data-a="cfSave" style="margin-top:14px;background:#ff4d00;color:#fff;height:54px;border-radius:27px;font:900 16px/1 var(--font-head)">${ic('plus',20,3)}${esc(t('mSave'))}</button></div><div class="tail"></div>`}
ACT.cfk=el=>{CF.k=el.dataset.id;render(true)};ACT.cfs=el=>{CF.sec=el.dataset.id;render(true)};ACT.cfc=el=>{CF.c=el.dataset.id;render(true)};
ACT.cfSave=()=>{const v=cfVal(),k=cfKind(),r=v?codeSvg(k,v):{err:'eEmpty'};if(r.err){toast(t(r.err));return}D.cards.push({id:'c'+uid(),n:CF.n.trim()||(CF.k==='wifi'?CF.ssid:kName(k)),k,v:k==='ean'?r.txt:v,c:CF.c});D.sel=D.cards[D.cards.length-1].id;save();CF={k:'qr',n:'',v:'',ssid:'',pw:'',sec:'WPA',c:'black'};tab='wal';Store.set(KEY+':tab',tab);render();$('#page').scrollTop=0;toast(t('saved2'))};
document.addEventListener('input',e=>{const id=e.target.id;if(!/^f[nvsp]$/.test(id||''))return;if(id==='fn')CF.n=e.target.value;else if(id==='fv')CF.v=e.target.value;else if(id==='fs')CF.ssid=e.target.value;else CF.pw=e.target.value;const pv=$('#pv');if(pv)pv.innerHTML=pvHTML()});

const NAV=()=>[{id:'wal',icon:'layers',label:t('nWal')},{id:'scan',icon:'camera',label:t('nScan')},{id:'make',icon:'grid',label:t('nMake')}];
const VIEWS={wal:vWal,scan:vScan,make:vMake};
function render(keep){const pg=$('#page'),y=keep?pg.scrollTop:0;pg.innerHTML=VIEWS[tab]();$('#nav').innerHTML=navHTML(NAV(),tab);pg.scrollTop=y}
ACT.tab=el=>{tab=el.dataset.id;Store.set(KEY+':tab',tab);render()};
render();
</script>
</body>
</html>
